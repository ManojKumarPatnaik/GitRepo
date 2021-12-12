package com.justdial.homepage;

import org.openqa.selenium.By;

import org.openqa.selenium.WebElement;


//Freelisting class 
public class Freelisting extends Homepage {
	public WebElement companyname, cityname, firstname, lastname, mobilenumber, landline, submit;

	//Method for finding webElements in Freelisting Page
	public void elements() {

		companyname = driver.findElement(By.name("cn"));
		cityname = driver.findElement(By.name("fcity"));
		firstname = driver.findElement(By.name("fname"));
		lastname = driver.findElement(By.name("lname"));
		mobilenumber = driver.findElement(By.name("mn[]"));
		landline = driver.findElement(By.name("ph"));
		submit = driver.findElement(By.xpath("//button[@class='bbtn subbtn']"));
	}
}
