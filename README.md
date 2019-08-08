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
- 函数规则
  * 函数不能抛出显性异常, 如下错误示范
    ```
      public void test() throw Exception{}
    ```
  * 禁止使用非必要性try catch, 如下示范
    ```
      public void test() {
        try {
          System.out.println("");
        } catch (Exception e) {
          e.printStackTrace();
        }
      }
    ```
  * 禁止使用日志输出方式
    ```
      System.out.println();
      e.printStackTrace();
    ```
    
  
  ```
    /**
     *  <函数具体使用说明>
     * @param name <参数说明>
     */
     public void test(String name){}
  ```
- 代码简洁规范
  * controll类禁止处理业务逻辑，遵循函数代码行越少越优原则
  * service业务处理类，尽量保证每个函数代码行数小于100为原则
  * 公共字符串尽量抽取枚举类或静态变量
   
- 代码空格使用
  * 类与实体之间只能使用一个空格
  * 参数之间只能使用一个空格
  * 括号内无需使用空格
  ```
    Test test = new Test();
    test.print("a", "b");
  ```
- 提交代码前必须使用```Ctrl+Shift+F```进行代码格式化

- SQL脚本规范
  * ${系统名称}\_${版本号}\_${日期}.sql
  * 脚本内容不能包含drop、delete、truncate命令
  * 所有脚本必须是增量脚本
  * 所有脚本必须包含业务注释，注明具体业务为什么需要执行此脚本
  
  
