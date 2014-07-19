SortDevelopers 19.07.2014 19:50
==============
package forDevelopers;

import java.util.*;

public class Main {
	public static void main(String[] args){
			Developer[] developers = new Developer[12];
    		developers[0] = new JuniorDeveloper(1, "Petr", 2300);
    		developers[1] = new SeniorDeveloper(2, "Dima", 1600);
    		developers[2] = new JuniorDeveloper(1, "Vova", 1050);
   			developers[3] = new SeniorDeveloper(2, "Jan", 1780);
    		developers[4] = new TeamLeadDeveloper(3, "Roman", 8900);
    		developers[5] = new SeniorDeveloper(2, "Mishka", 1000);
    		developers[6] = new SeniorDeveloper(2, "Kostia", 3400);
    		developers[7] = new JuniorDeveloper(1, "Oleg", 2590);
    		developers[8] = new SeniorDeveloper(2, "Oksana", 1600);
    		developers[9] = new SeniorDeveloper(2, "Jacov", 1400);
    		developers[10] = new TeamLeadDeveloper(3, "Rita", 6000);
    		developers[11] = new SeniorDeveloper(2, "Masha", 1200);  
Arrays.sort(developers);
                         
/* Печать отсортированных значений */
                         
for(int i = 0; i < developers.length; i++)
{
  System.out.println(developers[i].type + " "+
  developers[i].name + " " + developers[i].salary);
}
}
}

package forDevelopers;

import java.util.*;

public abstract class Developer implements Comparable {
	protected int type;
	protected String name;
	protected int salary;

	public Developer(int type, String name, int salary) {
		this.type = type;
		this.name = name;
		this.salary = salary;
	}

	public String getName() {
		return name;
	}

	public int getSalary() {
		return salary;
	}

	public abstract String printDeveloper();

	public int compareTo(Object obj) {
		Developer tmp = (Developer) obj;
		if (this.type < tmp.type) {
			/* текущее меньше полученного */
			return -1;
		} else if (this.type > tmp.type) {
			/* текущее больше полученного */
			return 1;
		}
		/* текущее равно полученному */
		return 0;
	}
}


package forDevelopers;

public class JuniorDeveloper extends Developer {
	public JuniorDeveloper(int type, String name, int salary) {
		super(type, name, salary);
	}
	
	@Override
	public String printDeveloper() {
		return name;
}
}


package forDevelopers;

public class SeniorDeveloper extends Developer {
	public SeniorDeveloper (int type, String name, int salary){
		super(type, name, salary);
	}
	
	@Override
	public String printDeveloper() {
			return name;
	}
}


package forDevelopers;

public class TeamLeadDeveloper extends Developer {
	public TeamLeadDeveloper(int type, String name, int salary) {
		super(type, name, salary);
	}
	
	@Override
	public String printDeveloper() {
		return name;
	}
}

