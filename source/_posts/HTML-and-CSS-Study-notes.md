---
title: HTML and CSS Study notes
date: 2017-03-24 23:25:08
tags:
---


HTML学习笔记（一）
First Day
超文本标记语言HTML:HyperText Markup Language;

1.匹配标记：开始标记和对应的结束标记；
2.标题、子标题、段落；
3.tag即标记无需在同一行：浏览器不关心制表符、回车、多个空格； 
4.body中包含的web页面的所有内容和结构，就是在浏览器中看到的部分；
5.编写HTML时要将首部（即head）和页面主体（即body）分开； 
6.有些元素（开始标记＋内容＋结束标记）会使用简写记法，即只有一个标记,如<img src="">;

Second Day
7.元素通过属性添加一些额外信息。

JAVA+WebDriver学习笔记（一）
/**
 * Return if the element is exists or not? 
 */
public boolean isElementPresent(By by) { 
try { driver.findElement(by); return true; 
} catch (NoSuchElementException e) { 
return false; }
} 

public By tableList = By.cssSelector(".data-table>tbody>tr"); 
isElementPresent(tableList); 

Second Day
/**
 * accept()必须在try外边
 */
public void delFeeSingle(){
    try{
    //点击：删除按钮
    feePaymentsListPage.delBtn_firstData.click();
    commonFuncs.sleep();
    }catch (UnhandledAlertException e){

    }

    //回车键
    driver.switchTo().alert().accept();
    commonFuncs.sleep();
}
