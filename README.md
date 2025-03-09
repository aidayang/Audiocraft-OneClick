# Audiocraft-OneClick
audiocraft文本转音乐软件免安装一键启动整合包
## Audiocraft官方介绍：
AudioCraft 是一个用于音频生成深度学习研究的 PyTorch 库。AudioCraft 包含两种最先进的 AI 生成模型的推理和训练代码，可生成高质量的音频：AudioGen 和 MusicGen。整合包我只制作了使用MusicGen模式的。

MusicGen：简单且可控制的音乐生成

AudioCraft 为 MusicGen 提供了代码和模型， MusicGen 是一种简单且可控的音乐生成模型。MusicGen 是一种单级自回归 Transformer 模型，通过 32kHz EnCodec 标记器进行训练，具有 4 个以 50 Hz 采样的码本。与MusicLM等现有方法不同，MusicGen 不需要自监督语义表示，并且它可以一次性生成所有 4 个码本。通过在码

本之间引入一个小的延迟，我们表明我们可以并行预测它们，因此每秒音频只有 50 个自回归步骤。我们使用 20,000 小时的授权音乐来训练 MusicGen。具体来说，我们依靠 10,000 首高品质音乐曲目的内部数据集以及 ShutterStock 和 Pond5 音乐数据。

## AudioCraft整合包使用方法说明
首先将网盘内的软件压缩包下载到本地电脑上并解压。双击启动软件.exe。稍等一会会自动打开webUI界面。整合包默认使用facebook/musicgen-stereo-melody模型，支持输入文本描述词和参考音乐素材。

先在input text里输入想要的音乐描述词英文单词，如果有参考音乐的话，可以在右侧选择音频文件，模型默认选facebook/musicgen-stereo-melody，Duration为合成音乐时长，默认10秒，最大120秒。其它参数可保持默认，点击按钮Submit即可生成音乐。

软件采用的是GPU计算模式，对电脑显卡有要求。

整合包里只预下载了musicgen-stereo-melody和musicgen-stereo-melody-large两种模型，musicgen-stereo-melody为质量和计算之间的最佳平衡，是官方推荐的模型。如果使用musicgen-stereo-melody-large模型，需要先到网盘里将这个模型压缩包下载到hf文件夹内并解压，然后才可使用。如果选择的模型本地电脑上没有的话，软件也会自动下载。

模型名中带stereo为可输出立体声音频。

模型名带melody为可输入参考音乐素材，也可以只输入文本描述词

如果电脑配置较高，Decoder可选择MultiBand_Diffusion，可以提高音频质量

视频教程及效果演示：[youtube>>](https://www.youtube.com/watch?v=crIV6UMcgOE)

## 注意事项
整合包只支持Windows10或11电脑，手机和mac无法使用

软件运行路径中不要出现非英文字符和空格，待使用的音频素材同样注意

Audiocraft并没有明确生成的音乐是否可以商用，大家在使用的时候请注意

## AI音乐生成器软件Audiocraft一键启动整合包下载：
https://pan.quark.cn/s/d62fa6fca7ac

## Audiocraft项目链接
https://github.com/facebookresearch/audiocraft
