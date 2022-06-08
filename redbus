package test12.test12;

import java.util.List;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import org.openqa.selenium.support.ui.Select;
import org.testng.Assert;
import org.testng.annotations.AfterTest;
import org.testng.annotations.BeforeSuite;
import org.testng.annotations.BeforeTest;
import org.testng.annotations.Test;

import net.bytebuddy.build.Plugin.Factory.UsingReflection.Priority;

public class Second {
	 public WebDriver driver;
	@BeforeTest
	  public  void Openbrowser() {
	
	System.setProperty("webdriver.chrome.driver", "E:\\chromedriver_win32 (6)\\chromedriver.exe");
	driver=new ChromeDriver();
	driver.manage().window().maximize();
}

	@Test()
	public void method1() {
		//Assert.fail();
		driver.get("https://www.redbus.in/");
	}
		@Test
		public void method3() {
			driver.findElement(By.xpath("//*[@id=\"src\"]")).sendKeys("Coi");
			
		
	}
		@Test
		public void method4() {
			List<WebElement> list =driver.findElements(By.xpath("//*[@id=\"search\"]/div/div[1]/div/ul/li[2]/descendant::i[@class='sub-city']"));
			System.out.println("number: "+ list.size());
			for(int i=0;i<list.size();i++) {
				System.out.println(list.get(i).getText());
			}
		
	}
@AfterTest
public void exit() throws InterruptedException {
	Thread.sleep(5000);
	driver.quit();
}
}	
