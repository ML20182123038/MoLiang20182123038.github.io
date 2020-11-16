 MoLiang20182123038

# Github Repositories 用例

## 一、用例分析与设计

### &nbsp;&nbsp;1、确定用例

&nbsp;&nbsp;&nbsp;&nbsp;（1）GitHub仓库系统有以下几类参与者：
- GitHub管理员
- 作者
- 用户<br>

&nbsp;&nbsp;&nbsp;&nbsp;（2）在上述参与者中，“作者”、“GitHub管理员”和“用户”实际分别通过各自控制台和键盘与仓库系统交互。通过这些参与者与仓库系统之间的交互场景进行归类和抽象，可以初步确定仓库系统应该具有以下用例，这些都是直接与外部参与者发生交互、对其可见的管理系统功能：
- 创建仓库
-  导入其他仓库
- 搜索仓库
- 选择仓库分支
- 上传仓库文件
- 创建文件
- 搜索文件
- 查看仓库详细描述信息
- 设置仓库
- 克隆仓库
- 管理查看仓库多种小功能<br>

## 二、生成用例图与用例描述
![Download](https://github.com/ycfxhsw/YangChunFu20182123027/blob/UML-Work/Download.png)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;图 2-1 GitHub仓库克隆

###  &nbsp;&nbsp;1、对 图 2-1Github仓库克隆的用例描述
用例名称：GitHub仓库克隆<br>
用例编号：Download.mdj<br>
用例说明：所有用户可以克隆作者公开的仓库，可以用仓库提供的clone连接下载，可以克隆到桌面应用程序阅读，还可以下载zip压缩包<br>
参与者：作者、管理员、用户<br>
前置条件：成功进入到仓库页面<br>
事件流：作者、GitHub管理员或者其他用户下载仓库文件<br>

![Management](https://github.com/ycfxhsw/YangChunFu20182123027/blob/UML-Work/Management.png)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;图 2-2 GitHub仓库管理
### &nbsp;&nbsp;2、对 图 2-2Github仓库管理的用例描述
用例名称：GitHub仓库管理<br>
用例编号：Management.mdj<br>
用例说明： 用户、作者、管理员可以使用的一些仓库公开功能<br>
参与者：作者、管理员、用户<br>
前置条件：成功进入到仓库页面<br>
事件流：<br>
（1）、GitHub管理员或者其他用户可以加入到作者仓库的编写开发中，通过Pull requests功能推送给仓库作者，作者通过后可以合并入作者仓库主分支。<br>
（2）、使用Actions：持续集成由很多操作组成，比如抓取代码、运行测试、登录远程服务器，发布到第三方服务等等。GitHub 把这些操作就称为 actions。很多操作在不同项目里面是类似的，完全可以共享。GitHub允许开发者把每个操作写成独立的脚本文件，存放到代码仓库，使得其他开发者可以引用。如果需要某个 action，不必自己写复杂的脚本，直接引用他人写好的 action 即可，整个持续集成过程，就变成了一个 actions 的组合。<br>
（3）、使用issues功能：<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;①发现软件的BUG并报告；<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;②有事想向作者询问、探讨；<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;③事先列出今后准备实施的任务。<br>
（4）、使用Wiki：其实可以替代README描述文件。<br>
（5）、通过insights查看自己仓库最近动态信息。<br>

![Setting](https://github.com/ycfxhsw/YangChunFu20182123027/blob/UML-Work/Setting.png)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;图 2-3 GitHub仓库设置
### &nbsp;&nbsp;3、对 图 2-3Github仓库设置的用例描述
用例名称：GitHub仓库设置<br>
用例编号：Setting.mdj<br>
用例说明：作者可以设置自己的仓库各种属性，包括删除仓库等等 <br>
参与者：作者<br>
前置条件：成功进入到仓库设置页面<br>
事件流：<br>
（1）、作者重命名自己的仓库。<br>
（2）、作者使用仓库提供的数据连接、操作服务。<br>
（3）、描述自己仓库，编写仓库主题，突出仓库特征。<br>
（4）、对自己的仓库进行备份处理。<br>
（5）、作者设置自己的仓库分支展示页面的主题，通过GitHub Pages功能把其他域名链接到展示页面。<br>
（6）、作者对自己的仓库进行危险操作，包括删除仓库、改变仓库可见属性、转移仓库所有权等。<br>

![Repositories](https://github.com/ycfxhsw/YangChunFu20182123027/blob/UML-Work/Repositories.png)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;图 2-4 GitHub仓库用例图
### &nbsp;&nbsp;4、对 图 2-4Github仓库用例描述
用例名称：GitHub仓库<br>
用例编号：Repositories.mdj<br>
用例说明：作者能够 使用仓库所有功能，其他用户只够使用仓库一部分功能<br>
参与者：作者、管理员、用户<br>
前置条件：作者创建好仓库，并成功进入到仓库页面<br>
事件流：<br>
（1）、所有用户能够克隆仓库。<br>
（2）、所有人查看仓库代码、文件、仓库描述信息。<br>
（3）、所有人能够选择仓库分支。<br>
（4）、所有用户能够把其他人的仓库拉取到自己仓库中。<br>
（5）、其他人参与仓库项目的编写然后推给作者，如果作者同意可以合并入作者的分支。<br>
（6）、作者上传文件。<br>
（7）、其他用户可以创建文件，上传后需要作者通过。<br>
（8）、搜索仓库文件。<br>
（9）、作者设置自己的仓库属性。<br>
