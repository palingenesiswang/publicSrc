# flutter 错误锦集

- [ERROR:flutter/shell/gpu/gpu_surface_gl.cc(58)\] Failed to setup Skia Gr context

  ![](https://img2018.cnblogs.com/blog/939316/201905/939316-20190529104409691-554197625.png)

  ```dart
  flutter run --enable-software-rendering
  ```

- [ERROR:flutter/shell/gpu/gpu_surface_gl.cc(70)] Failed to setup Skia Gr context.
  Error connecting to the service protocol: failed to connect to http://127.0.0.1:6511/tEC-2Vjr4H4=/

  ![](https://user-images.githubusercontent.com/7868514/65825540-6ea2ee00-e2aa-11e9-9988-34b87d3837c8.png)

  > 跟上面问题一样，但这是MuMu模拟器的锅，解决方案如下：
  
  ```dart
flutter run --enable-software-rendering
  ```
  
  > 出来选项选择热重启即可，但没办法使用AS自带的run 及debug；
  >
  > 在MuMu模拟器找到设置->高级设置->显卡渲染模式改成**兼容+(openGL)**即可

