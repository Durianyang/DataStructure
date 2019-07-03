### 策略模式与命令模式区别


1. 策略模式 定义一系列算法，把它们一个个封装起来，并且使它们可以相互替换。该模式使得算法可独立于它们的客户变化。

2. 将一个请求封装为一个对象，从而使你可用不同的请求对客户进行参数化；对请求排队或记录请求日志，以及支持可撤销的操作。 



我个人觉得，策略模式和命令模式的其中一个最大区别，
是在于：策略模式对付的问题域通常是一个，就是说，多个策略只是处理同一个问题，比如排序问题，使用不同的排序算法

而命令模式对付的是多个问题域，就是很多不同的命令来做不同的事情。 比如关机  开启 命令，开机和关机 是两种不同的事情

再比如，关机时，有程序没退出（可以采用一个一个退出的算法退出），也可以（采用直接杀死所有程序的方式）


比如  让机器人去跑步  和 吃饭  是命令模式，因为干的不一样的事，跑步 的路径选着  是策略模式  



3. 如果是播放不同类型音乐，应该是命令模式，接收到不同的命令后去播放不同类型的音乐，同时还需要一个接收者知道播放的进度


更多的情况命令模式比策略模式多了一个接收者