# leitingzhanji
MVC design

import java.awt.Graphics;
import java.awt.Image;

import javax.swing.ImageIcon;

/****
 * 子弹类 
 * @author Adminstators
 *
 */
public class Bullet {
	
	private int x ;
	private int y;
	private int r;
	private Image bulletImage = new ImageIcon("img/fire.png").getImage();
	
	//设置 子弹属性的方法
	public int getX() {
		return x;
	}
	public void setX(int x) {
		this.x = x;
	}

	public int getY() {
		return y;
	}
	public void setY(int y) {
		this.y = y;
	}
	public int getR() {
		return r;
	}
	public void setR(int r) {
		this.r = r;
	}
	
	
	//绘制方法
	
	public void paint (Graphics g) {
		g.drawImage(bulletImage, x - r - 15, y - r - 100, null);
	}
	
	

}
