Chapter 4 集合
集合 或 容器 是 Java 中存放数据的重要数据结构

字符串 java.lang.String
字符串初始化后，其值不能改变 immutable

String 的重要(成员)方法
1.**charAt**  
   -  char|charAt(int index) 
   - 返回指定索引处的 char 值。
2.**concact**  concatenate[kɒn'kætɪneɪt]
   - String |concat(String str) 
   - 将指定字符串连接到此字符串的结尾。
3.**contains** 
   - boolean|contains(CharSequence s) 
   - 当且仅当此字符串包含指定的 char 值序列时，返回 true。
**endsWith**
    boolean|endsWith(String suffix) 
    测试此字符串是否以指定的后缀结束。
**equals** 
    boolean|equals(Object anObject) 
    将此字符串与指定的对象比较。
**equalsIgnoreCase** 
    boolean|equalsIgnoreCase(String anotherString) 
    将此 String 与另一个 String 比较，不考虑大小写。
**format**
    static String|format(Locale l, String format, Object... args) 
    使用指定的语言环境、格式字符串和参数返回一个格式化字符串。
**getBytes** 
    byte[]	|getBytes() 
    使用平台的默认字符集将此 String 编码为 byte 序列，并将结果存储到一个新的 byte 数组中。
    byte[]	|getBytes(Charset charset) 
    使用给定的 charset 将此 String 编码到 byte 序列，并将结果存储到新的 byte 数组。
    byte[]	|getBytes(String charsetName) 
    使用指定的字符集将此 String 编码为 byte 序列，并将结果存储到一个新的 byte 数组中。         
**indexOf** 
    int	|indexOf(int ch) 
    返回指定字符在此字符串中第一次出现处的索引。
    int	|indexOf(int ch, int fromIndex) 
    返回在此字符串中第一次出现指定字符处的索引，从指定的索引开始搜索。
    int |indexOf(String str) 
    返回指定子字符串在此字符串中第一次出现处的索引。
    int	|indexOf(String str, int fromIndex) 
    返回指定子字符串在此字符串中第一次出现处的索引，从指定的索引开始。
**isEmpty** 
    boolean	|isEmpty() 
    当且仅当 length() 为 0 时返回 true。
**lastIndexOf** 
    int	|lastIndexOf(int ch) 
    返回指定字符在此字符串中最后一次出现处的索引。
    int	|lastIndexOf(int ch, int fromIndex) 
    返回指定字符在此字符串中最后一次出现处的索引，从指定的索引处开始进行反向搜索。
    int	|lastIndexOf(String str) 
    返回指定子字符串在此字符串中最右边出现处的索引。
    int	|lastIndexOf(String str, int fromIndex) 
    返回指定子字符串在此字符串中最后一次出现处的索引，从指定的索引开始反向搜索。
**length** 
    int	|length() 
    返回此字符串的长度。
**matches** 
    boolean	|matches(String regex) 
    告知此字符串是否匹配给定的正则表达式。
**replace** 
    String	|replace(char oldChar, char newChar) 
    返回一个新的字符串，它是通过用 newChar 替换此字符串中出现的所有 oldChar 得到的。
    String	|replace(CharSequence target, CharSequence replacement) 
    使用指定的字面值替换序列替换此字符串所有匹配字面值目标序列的子字符串。
**replaceAll** 
    String	|replaceAll(String regex, String replacement) 
    使用给定的 replacement 替换此字符串所有匹配给定的正则表达式的子字符串。
**replaceFirst** 
    String	|replaceFirst(String regex, String replacement) 
    使用给定的 replacement 替换此字符串匹配给定的正则表达式的第一个子字符串。
**split** 
    String[] |split(String regex) 
    根据给定正则表达式的匹配拆分此字符串。
    String[] |split(String regex, int limit) 
    根据匹配给定的正则表达式来拆分此字符串。
**startWith** 
    boolean	|startsWith(String prefix) 
    测试此字符串是否以指定的前缀开始。
    boolean	|startsWith(String prefix, int toffset) 
    测试此字符串从指定索引开始的子字符串是否以指定前缀开始。
**subString** 
    String	|substring(int beginIndex) 
    返回一个新的字符串，它是此字符串的一个子字符串。
    String	|substring(int beginIndex, int endIndex) 
    返回一个新字符串，它是此字符串的一个子字符串。
**toCharArray** 
    char[]	|toCharArray() 
    将此字符串转换为一个新的字符数组。
**toLowerCase** 
    String	|toLowerCase() 
    使用默认语言环境的规则将此 String 中的所有字符都转换为小写。
    String	|toLowerCase(Locale locale) 
    使用给定 Locale 的规则将此 String 中的所有字符都转换为小写。
**toUpperCase** 
    String	|toUpperCase() 
    使用默认语言环境的规则将此 String 中的所有字符都转换为大写。
    String	|toUpperCase(Locale locale) 
    使用给定 Locale 的规则将此 String 中的所有字符都转换为大写。
**trim**
    String	|trim() 
    返回字符串的副本，忽略前导空白和尾部空白。
**valueOf**
    static String   |valueOf(boolean b) 
    返回 boolean 参数的字符串表示形式。
    static String	|valueOf(char c) 
    返回 char 参数的字符串表示形式。
    static String	|valueOf(char[] data) 
    返回 char 数组参数的字符串表示形式。
    static String	|valueOf(char[] data, int offset, int count) 
    返回 char 数组参数的特定子数组的字符串表示形式。
    static String	|valueOf(double d) 
    返回 double 参数的字符串表示形式。
    static String	|valueOf(float f) 
    返回 float 参数的字符串表示形式。
    static String	|valueOf(int i) 
    返回 int 参数的字符串表示形式。
    static String	|valueOf(long l) 
    返回 long 参数的字符串表示形式。
    static String	|valueOf(Object obj) 
    返回 Object 参数的字符串表示形式。
字符串缓冲区 java.lang.StringBuffer
append 
delete 
insert 
reverse 
setCharAt