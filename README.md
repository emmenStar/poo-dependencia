# poo-dependencia
package aaaaaaaaaa;
//interface grafica

import java.awt.Button;
import java.awt.Container;
import java.awt.FlowLayout;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

import javax.swing.JButton;
import javax.swing.JFrame;
import javax.swing.JOptionPane;

public class Eminsi extends JFrame  implements ActionListener {
	public Eminsi() {
		setTitle("eminsi");
		setDefaultCloseOperation(EXIT_ON_CLOSE); 
		setSize(420, 350);
		Container container = getContentPane();
		container.setLayout(new FlowLayout());
		
		JButton button = new JButton("clique aqui");
		button.addActionListener(this);
		container.add(button);
		
		JButton button2 = new JButton("clique aqui");
		button2.addActionListener(this);
		container.add(button2);
		
	}
	
	@Override
	public void actionPerformed(ActionEvent e) {
			
		if (e.getSource() == button) {
			JOptionPane.showConfirmDialog(null, "anaBanna");			
		}
		if (e.getSource() == button2) {
			JOptionPane.showConfirmDialog(null, "anaBannaChicleteBacana");			
		}		
		
	}
	public static void main(String [] args) {
		Eminsi e = new Eminsi();
		e.setVisible(true);
	}
}

extra

package src;

import java.awt.event.MouseEvent;
import java.awt.event.MouseMotionListener;

import javax.swing.JFrame;

public class Janela extends JFrame {
	
	public Janela(){
		
		setTitle("");
		setSize(500,500);
		setDefaultCloseOperation(EXIT_ON_CLOSE);
		
		addMouseMotionListener(new MouseMotionListener(){
			
		public void mouseMoved(MouseEvent e) {
		int x = e.getX();
		int y = e.getY();
		System.out.println(x + "-" + x);
	}
		public void mouseDragged(MouseEvent e) {
			
		}
	});

	}
}
