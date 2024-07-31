# XiDiarrhoea - 一款 Minecraft 拉肚子插件

**XiDiarrhoea** 是一款让你的玩家不再轻视生食的 Minecraft 插件。该插件通过模拟消化不适，增加了游戏的真实性和挑战性。

## 简介

在原版 Minecraft 中，吃生食只会造成轻微的饥饿效果。而 XiDiarrhoea 插件将此效果拓展，引入了一系列有趣的后果：

1. **不适感**：玩家吃下某些食物后会感到肚子不舒服。
2. **拉肚子状态**：进入拉肚子状态后，玩家必须找到水源并蹲下“释放”。
3. **意外事件**：如果玩家在行走时蹲下，则会“拉裤子”，并出现棕色粒子效果，必须进入水中才能清除。
4. **死亡机制**：如果玩家长时间不解决问题，将因憋屎过久而死亡，并触发全服公告。
5. **与 XiFart 的联动**：如果同时安装了 XiFart 插件，还可以触发更多的崩屎效果，并进行全服公告。

### 功能

- **可自定义效果**：可以配置药水效果、消息和时间。
- **死亡和提醒**：自定义玩家憋屎的最长时间，并设置提醒消息。
- **与 XiFart 插件联动**：利用 XiFart 插件增强游戏趣味性。

## 安装

1. 下载 XiDiarrhoea 的最新版本。
2. 将 JAR 文件放入 Minecraft 服务器的 `plugins` 目录中。
3. 启动服务器以生成默认配置文件。

## 配置

```yaml
# config.yml

water-check-rate: 20
poop-check-rate: 20
particle-check-rate: 5
xifart-shit-rate: 600

diarrhea-death-duration: 30
diarrhea-warning-threshold: 10
diarrhea-warning-message: "&c你将在 %seconds% 秒后因拉肚子死亡！"

potion-effects:
  - WEAKNESS
  - SLOW

prefix: "&7[&6XiDiarrhoea&7]"

messages:
  discomfort: "&e你感到肚子不舒服..."
  release: "&e可以释放自己了，快点，夹不住了！"
  pooped: "&e没有水源！你拉裤子了！"
  success: "&e你成功缓解了窜稀症状！"
  death: "&e憋尿能行千里 拉屎寸步难行 玩家 &l&e%player% &e因为憋屎太久 &4死了"

diarrhea-causing-items:
  - ROTTEN_FLESH
  - POISONOUS_POTATO
  - SPIDER_EYE
  - PORK
  - BEEF
  - CHICKEN
  - MUTTON
  - RABBIT
  - COD
  - SALMON
  - TROPICAL_FISH
  - PUFFERFISH
  - RAW_MUTTON
  - RAW_RABBIT
  - RAW_COD
  - RAW_SALMON
  - RAW_CHICKEN
  - RAW_BEEF
  - RAW_PORK
  - POTATO
  # 可以在这里添加更多的食物类型
