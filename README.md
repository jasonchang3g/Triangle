import java.awt.Color;
import java.awt.Dimension;
import java.awt.event.MouseEvent;
import java.awt.event.MouseListener;
import java.awt.Font;
import java.awt.Graphics;
import java.awt.Graphics2D;
import java.awt.Point;
import javax.swing.JFrame;
import javax.swing.JPanel;
import java.awt.event.MouseListener;
import java.awt.event.MouseEvent;
import javax.swing.JFrame;
import java.awt.event.KeyListener;
import java.awt.event.KeyEvent;
import java.awt.geom.Point2D;
import javax.swing.KeyStroke;


public class Triangle extends JFrame
{
   private static final int FRAME_WIDTH = 300;
   private static final int FRAME_HEIGHT = 400;
   

   private Triangle scene;

   class MousePressListener implements MouseListener
   {  
      public void mousePressed(MouseEvent event)
      {
    	  Point2D.Double point = new Point2D.Double(event.getX(), event.getY());
    	  }

      public void mouseReleased(MouseEvent event) {}
      public void mouseClicked(MouseEvent event) {}
      public void mouseEntered(MouseEvent event) {}
      public void mouseExited(MouseEvent event) {}
   }


public void RectangleFrame()
{
   scene = new Triangle();
   add(scene);

   MouseListener listener = new MousePressListener();
   scene.addMouseListener(listener);

  

   setSize(FRAME_WIDTH, FRAME_HEIGHT);
}
} 
