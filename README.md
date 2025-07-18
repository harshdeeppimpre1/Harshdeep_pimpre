package pageObjects;

import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.support.FindBy;

public class HomePage extends BasePage {

	WebDriver driver;

	public HomePage(WebDriver driver) {

		super(driver);

	}

	@FindBy(xpath = "//span[normalize-space()='My Account']")WebElement LnkMyAccount;
	@FindBy(xpath = "//li//ul//a[text()='Register']")WebElement LnkRegister;

	public void ClickMyAccount() {
		LnkMyAccount.click();
	}

	public void ClickRegister() {
		LnkRegister.click();

	}

}
