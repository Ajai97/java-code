package collectionlab1;
import java.util.*;

class book{
	String name;
	book(String a){
		name=a;
	}
	void display() {
		System.out.println(name);
	}	
}

public class ArrayList1 {

	public static void main(String[] args) {
		ArrayList<String>  l=new ArrayList<String>  ();
		l.add("book1");
		l.add("book2");
		l.add("book3");
		l.add("book4");
		l.add("book5");
	Iterator i=l.iterator();
	while(i.hasNext()) {
		System.out.println(i.next());
	}
		ArrayList <book> b=new ArrayList<book>();
		book p1=new book("Harry Potter");
		book p2=new book("Harry Potter and Prisoner of Azkaban");
		book p3=new book("Harry Potter and Goblit of fire ");
		book p4=new book("Harry Potter and Secret of Chamber");
		book p5=new book("Harry Potter and Deathly hollow");
		
		b.add(p1);
		b.add(p2);
		b.add(p3);
		b.add(p4);
		b.add(p5);
		for (book p:b) {
			System.out.println(p.name);
		}
		
		
	}

}
