# <center> 第一章
## 一、课后作业 
### 1、文件组织
![](./Picture/ch2/p1.png)     
&emsp;&emsp;在JAVA Project ch2中，我新建了一个homework包，其中有一个主类Main用来测试其他类中的方法和函数，另外还有两个类Math和Month用来实现题目要求功能。
###2、题目实现
####（1）输入一个月份，然后输出对应的月份有多少天(不考虑闰年)，将天数输出。
&emsp;&emsp;以下为Month类及monthData方法的代码。
    /**
     * 
     */
    package homework;
    
    /**
     * @author forest
     *
     */
    public class Month 
    {
    
    	/**
    	 * 
    	 */
    	public static short monthDate(short month) 
    	{
    		short month_arry[] = {31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31};
    		
    		return month_arry[month-1];
    	}
    }
&emsp;&emsp;本题采用数组存放了12个月的天数，通过查找的方式找到每个月的天数。