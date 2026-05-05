# TMUX Config

个人 TMUX 配置备份 - Nord 主题 + 系统监控

## 特性

- 🎨 **Nord 配色方案** - 舒适的颜色主题
- 📊 **系统监控** - CPU/内存实时显示 (4 秒刷新)
- ⚡ **Vim 风格快捷键** - 高效的窗格操作
- 🔌 **TPM 插件支持** - 易于扩展
- 📝 **会话持久化** - 自动保存/恢复

## 预览

```
状态栏:
 thorn | 1:zsh 2:nvim 3:tmux   CPU 25%   MEM 4.2GB  🕒 14:30  📅 2026-05-05
```

## 快速开始

### 1. 克隆配置
```bash
git clone git@github.com:kuku-199/tmux-config.git
cd tmux-config
```

### 2. 安装 TPM 插件
```bash
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

### 3. 链接配置
```bash
ln -sf $(pwd)/.tmux.conf ~/.tmux.conf
```

### 4. 安装插件
启动 tmux 后按 `Prefix + I` (Ctrl+b, 然后大写 I)

## 快捷键

| 快捷键 | 功能 |
|--------|------|
| `Ctrl+b, r` | 重新加载配置 |
| `Ctrl+b, c` | 新建窗口 |
| `Ctrl+b, \|` | 左右分割 |
| `Ctrl+b, -` | 上下分割 |
| `Ctrl+b, [` | 复制模式 |
| `Ctrl+b, P` | 粘贴 |

### 复制模式
1. `Ctrl+b, [` 进入复制模式
2. `v` 开始选择
3. `y` 或 `Enter` 复制
4. `Ctrl+b, P` 粘贴

## 配置

- **前缀键**: `Ctrl+b`
- **状态栏位置**: 底部
- **更新间隔**: 4 秒
- **终端图标**: `` (需要 Nerd Fonts)

## 插件

- [TPM](https://github.com/tmux-plugins/tpm) - 插件管理器
- [vim-tmux-navigator](https://github.com/christoomey/vim-tmux-navigator) - Vim 导航
- [tmux-resurrect](https://github.com/tmux-plugins/tmux-resurrect) - 会话保存
- [tmux-continuum](https://github.com/tmux-plugins/tmux-continuum) - 自动保存
- [tmux-cpu-mem-monitor](https://github.com/hendrikmi/tmux-cpu-mem-monitor) - 系统监控

## 字体

需要安装 **Nerd Fonts** 以显示图标：
- 下载：https://www.nerdfonts.com/
- 推荐：JetBrains Mono Nerd Font, Fira Code Nerd Font

## License

MIT
