# 24 质量管理

- [24 质量管理](#24-%E8%B4%A8%E9%87%8F%E7%AE%A1%E7%90%86)
  - [24.1软件质量](#241%E8%BD%AF%E4%BB%B6%E8%B4%A8%E9%87%8F)
  - [24.2 软件标准](#242-%E8%BD%AF%E4%BB%B6%E6%A0%87%E5%87%86)
  - [24.3 复查与审查](#243-%E5%A4%8D%E6%9F%A5%E4%B8%8E%E5%AE%A1%E6%9F%A5)
  - [24.4 软件度量和量度](#244-%E8%BD%AF%E4%BB%B6%E5%BA%A6%E9%87%8F%E5%92%8C%E9%87%8F%E5%BA%A6)

- 质量保证团队：在大多数公司负责管理版本测试过程，即负责软件的测试，检查系统是否满足需求，以及维护测试过程记录
- 质量规划：为项目制定一个质量计划的过程。应当列出要达到的软件质量，并且描述怎么评估这些质量
- 质量文档：记录项目中的每个子小组所做的工作的文件
  - 帮助检查，以避免遗忘重要的任务，或避免团队的一部分会对其他团队所做的工作做出错误的假设
  - 贯穿一个系统生命周期的沟通手段
  - 允许对系统进化负责的小组追踪测试以及开发团队所做的工作

## 24.1软件质量

- 软件质量管理的一个通用假设：按照需求测试系统。根据测试结果判断是否实现了要求的功能
- 系统的主观质量很大部分依赖于非功能特性：安全性、可理解性、可移植性、信息安全性、可测试性、可用性、可靠性、可调节性、可复用性、适应力、模块化、效率、鲁棒性、复杂度、学习能力
- 开发过程对于软件质量有明显的影响：好的过程更有可能得到好的软件。过程质量的管理和改进能够减少软件开发过程中产生的缺陷

## 24.2 软件标准

重要性 | 描述
--- | ---
智慧的结晶 | 软件标准封装了对于机构来说最成功的或最恰当的软件开发实践。制定为标准可避免重犯错误
为定义特定环境中的“质量”含义提供了一个框架 | 通过使用标准，为判断软件是否达到要求的质量水平建立基础
有助于工作的连续性 | 由一个人着手进行的工作别人可以接着做。软件标准确保一个机构中所有的工程人员采用相同的做法

类型 | 描述
--- | ---
产品标准 | 用于开发的软件产品。包括文档标准，如需求文档格式，文档编写标准，编码标准
过程标准 | 定义了软件开发必须遵循的过程。应将良好的开发方法封装其中。过程标准包括对描述、设计和有效性验证过程、过程支持工具以及对在这些过程中产生的文档的描述的定义

- 为了减少不满情绪，设定标准的质量管理人员要采取以下步骤
  - 让软件工程人员参与产品标准的选择
  - 定期评审和修改标准，以反映技术的变化
  - 尽可能提供支持软件标准的软件工具

## 24.3 复查与审查

- 质量复查：检查文档和代码的一致性和完整性，确保遵循质量标准
  - 用来发现软件和项目文档的问题和遗漏
  - 复查的结果应当作为质量管理过程的一部分被正式记录
- 过程复查：将软件工程的实际过程和计划过程对比。关注点是工程是否能够按时并在预算范围内发布有用的软件
- 复查和审查的目的是提升软件的质量，不是评估开发团队成员的表现
  - 项目管理人员必须对个人的关注保持敏感。必须营造一种文化，发现错误时不责备当事人
- 复查过程
  - 1 复查前活动：复查前工作关心复查的计划和复查的准备工作
    - 复查计划：包括建立一个复查团队，安排复查的时间地点，分发要被复查的文档
    - 复查准备工作：复查团队见到要复查的软件的一个综述
      - 部分复查团队成员需要阅读并理解软件、文档及相关标准
      - 他们独立工作，依靠标准找出错误、遗漏和违背的地方
      - 不能参加会议的复查人员，可以提供书面的软件意见
  - 2 复查会议：会议期间，被复查文档或程序的作者和复查团队一起把文档从头到尾浏览一遍
    - 复查时间不超过两个小时
    - 包含一个复查主席，负责保证所有的书面意见被考虑在内。在复查期间写西安一个达成共识的意见和行动的记录
    - 包含一个成员正式记录所有复查决议和要采取的行动
  - 3 复查后活动：会议结束后，必须解决在复查期间提出的问题
    - 比如修复软件漏洞，重构软件以使它和质量标准一致，重写文档
- 敏捷过程的复查
  - Scrum：每次迭代完成后，会有一个复查会议(冲刺复查)，讨论质量问题
  - 极限编程：配对编程确保另一个团队成员经常检查和复查代码。极限编程依赖于个人主动性来提升和重构代码
- 程序审查：同行评审，团队成员合作发现开发程序中的漏洞
  - 不同背景的团队成员，对程序源码进行精心、一行一行的复查
  - 寻找错误和问题(逻辑错误，代码异常等)，并在审查会议中描述出来
  - 审查时，经常使用一份常见编程错误的检查表。且不同的语言有不同的检查表
  - 每个机构应当根据部门标准和实践开发自己的检查表，并经常更新检查表

## 24.4 软件度量和量度

中文 | 英文 | 描述 | 目标
--- | --- | --- | ---
软件度量 | measurement | 对软件组织、系统或过程的某种属性进行量化 | 长期目标是利用度量代替复查，评判软件质量。度量之后达到所需质量阈值就可以不通过复查而被接受
软件量度 | metric | 能被客观度量的软件系统、系统文档或开发过程有关的特性 | 软件量度影响管理决策的制度

软件量度分类 | 描述 | 举例 | 影响
--- | --- | --- | ---
控制量度 | 支持过程管理，常与软件过程相关 | 修复发现的缺陷所需平均工作量和时间 | 决定是否做出过程改变
预言者量度(产品量度) | 与软件本身相关 | 模块的回路复杂性，程序中标识符的平均长度，在设计中与对象有关的属性和操作的数量 | 用来估计软件变更所需的成本

- 软件产品量度可能用到的方法：
  - 给系统质量属性赋值：通过度量系统组件的特性(如回路复杂性)，并综合这些量度，评估系统质量属性(如可维护性)
  - 找出质量低于标准的系统组件：度量能识别哪些特性背离某些规范的个别组件。比如找出有着高复杂性的问题组件，因为复杂度高难于理解，组件更可能包含错误

- CK 面向对象的量度套件

面向对象量度 | 描述
--- | ---
每个类加权后的方法 | 每个类的方法数，是对每个方法根据复杂度进行加权后计算所得。度量值越大，对象类越复杂
继承树的深度(DIT) | 在继承树中的具体层数。继承树越深，设计越复杂
孩子数(NOC) | 度量类的直接子类数，NOC 度量类层次结构的宽度，DIT 代表它的深度。NOC 高意味着更多的复用
对象类间耦合度(CBO) | 当一个类中的方法使用在另一个类中定义的方法或实例时，类间就是耦合的。CBO 意味着类是高度依赖的
对类的响应(RFC) | 当类的对象接收到消息时潜在可能的对此做出相应的方法数的度量。RFC 越高，类的复杂度越高
方法追你个缺乏内聚力(LCOM) | 通过计算类中各对方法而得。LCOM 是两个数的差，一个数是方法间没有共享属性的方法对数，一个数是方法间共享属性的方法对数。此亮度值的意义有争议

- 软件组件分析的关键阶段
  - 选择要做的度量
  - 选择要评估的组件
  - 度量组件特性
  - 识别异常度量
  - 分析异常组件
