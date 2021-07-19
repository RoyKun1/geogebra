# Commands and Undo-Points

- `boolean evalCommand(String cmdString)`：
  - 从3.0版开始维护
  - 评估给定的字符串，就像在输入 GeoGebra 的输入栏中时评估给定的字符串一样。 返回命令评估是否成功
  - 3.2 开始，可以通过用 \n 分隔来一次传递多个命令
- `String[] evalCommandGetLabels(String cmdString)`
  - 从5.0版开始维护
  - 返回以顿号分隔的创建对象的标签列表，例如“A、B、C”
- `String evalCommandCAS(String string)`
  - 从3.2版开始维护
  - 将字符串传递给 GeoGebra 的 CAS 并将结果作为字符串返回
- `void setUndoPoint()`
  - 设置撤销点。 如果您希望用户能够撤消 evalCommand 的操作，例如，如果您制作了一个 HTML 按钮作为自定义工具，则很有用

