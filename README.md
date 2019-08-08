# LOEX 编码规范

### 代码规范
- 类顶部必须带有注释
  ```
  /**
   *  <类用途>
   * @author <作者>
   * @since <时间>
   */
   public class Test {}
   ```
- 代码空格使用
  * 类与实体之间只能使用一个空格
  * 参数之间只能使用一个空格
  * 括号内无需使用空格
  ```
    Test test = new Test();
    
    test.print("a", "b");
  ```
- 提交代码前必须使用```Ctrl+Shift+F```进行代码格式化
