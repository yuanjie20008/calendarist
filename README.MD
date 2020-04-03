# 日期计算家，可实现阳历、阴历、干支历的相互转换


![maven](https://img.shields.io/maven-central/v/org.hothub/requestclient.svg)
![license](https://img.shields.io/github/license/opprime/requestclient.svg)


## 使用方法
>Maven引用
```
    <dependency>
        <groupId>org.hothub</groupId>
        <artifactId>calendarist</artifactId>
        <version>1.0.0</version>
    </dependency>
```

## 功能介绍
1. 阳历时间转阴历时间
2. 阴历时间转阳历时间
3. 阳历时间转干支时间
4. 阴历时间转干支时间

## 代码示例：

### 阳历转阴历：
```
LunarCalendarist calendarist = Calendarist.fromSolar(2020, 1, 1, 12, 15, 55, 58);
LunarDate lunarDate = calendarist.toLunar();
```

### 阳历转干支：
```
LunarCalendarist calendarist = Calendarist.fromSolar(2020, 1, 1, 12, 15, 55, 58);
LunarDate lunarDate = calendarist.toLunar();
```

### 阴历转阳历：
```
SolarCalendarist calendarist = Calendarist.fromLunar(2020, 1, 1, 12, 15, 55, 58);
SolarDate solarDate = calendarist.toSolar();
```