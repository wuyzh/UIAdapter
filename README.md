# UIAdapter
###传统dp适配方式的缺点
android中的dp在渲染前会将dp转为px，计算公式：
- px = density * dp;
- density = dpi / 160;
- px = dp * (dpi / 160);

而dpi是根据屏幕真实的分辨率和尺寸来计算的，每个设备都可能不一样的。

支持以宽或者高一个维度去适配，保持该维度上和设计图一致；

###找兼容突破口
从dp和px的转换公式 ：px = dp * density
