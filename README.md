# swooptest
Created scripts using Salenium using Eclipse IDE.
Programming lanuage used is JAVA.
Verified google flights page by printing Title of the page.
Used Chrome browser to execute this test case.

Script::
package swoopTest;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class SearchFlights {
	

	public static void main(String[] args) throws InterruptedException {
		String url = "https://www.google.com/flights";
		
		WebDriver driver = new ChromeDriver();
		
		System.setProperty("webdriver.chrome.driver","c:\\chromedriver.exe");
		
		driver.get(url);
		
		driver.manage().window().maximize();
		
		Thread.sleep(1000);	
		
		String Title = driver.getTitle();
		
		System.out.println(Title);

	}

}
