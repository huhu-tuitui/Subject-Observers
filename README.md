# Subject-Observers
模式设计基本原则：将变化部分与固定不变的部分相分离。

观察者模式
观察者模式定义了对象间的一对多依赖关系。
当一方的对象改变状态时，所有的依赖者都会被通知并自动被更新。

1.WeatherData类定义了获得温度、湿度和气压的方法；
2.只要有新的气象数据measurementsChanged()方法就会被调用；
3.我们需要使用气象数据来提供三种报告，并且，每当weatherData有新的数据是这三种报告就要更新；
4.我们要开发的系统必须是可扩展的。其他开发者可以建立定制的报告，用户可以随意增减他们需要的报告。目前，我们只知道三种报告类型：当前天气情况，气象统计报告，天气预报。
