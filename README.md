# My-first-Program
Assignment!
package in.kletech.minor;

public class minor {

	private int programCode;
	private String sSchoolCoordinator;
	int noOfStud;
	int noOfStaff;
	static int iSid;
	static int iSid1;
	static int iSid2;
	private final String cetcode1 = "E241";
	private final String cetcode2 = "E30";

	public static int getProgramCode() {
		return programCode;
	}

	public String getsSchoolCoordinator() {
		return sSchoolCoordinator;
	}

	public int getNoOfStud() {
		return noOfStud;
	}

	public int getNoOfStaff() {
		return noOfStaff;
	}

	public String getCetcode1() {
		return cetcode1;
	}

	public String getCetcode2() {
		return cetcode2;
	}

	public minor(String sSchoolCoordinator, int noOfStud, int noOfStaff) {
		// super();
		// iSid++;
		// System.out.println("The student id : "+iSid);
		this.sSchoolCoordinator = sSchoolCoordinator;
		this.noOfStud = noOfStud;
		this.noOfStaff = noOfStaff;
	}

	void create(int pcode) {
		if (pcode == 1) {
			iSid++;
			System.out.println("Student  :" + iSid);
			System.out.println("Electronics and Communication");

		}
		if (pcode == 2) {
			iSid1++;
			System.out.println("Student   :" + iSid);
			System.out.println("Computer Science");
		}
		if (pcode == 3) {
			iSid2++;
			System.out.println("Student   :" + iSid);
			System.out.println("Mechanical Engineering");
		}
	}

	void intake(int noOfStud) {
		if (noOfStud >= 120)
			System.out.println("Seats Full!!");
		else
			System.out.println("Seats Availaible");
	}

	void strength() {
		System.out.println();
		System.out.println(" Electronics and Communication:" + iSid);
		System.out.println();
		System.out.println(" Computer Science :" + iSid1);
		System.out.println();
		System.out.println(" Mechanical Engineering :" + iSid2);
		System.out.println();
	}

}
------------------------------------------------------------------------------
package in.kletech.minor;

public class minordemo {

	/**
	 * @param args
	 */
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		/*
		 * final string CET CODE1= "E30"; final string CET CODE2= "E241";
		 * System.out.println("CET CODE1");
		 */

		minor m1 = new minor(null, 1, 50);
		m1.create(1);
		m1.intake(50);
		System.out.println("_____________________________________________");
		minor m2 = new minor(null, 3, 150);
		m2.create(3);
		m2.intake(150);
		System.out.println("_____________________________________________");
		minor m3 = new minor(null, 2, 60);
		m3.create(2);
		m3.intake(60);
		System.out.println("_____________________________________________");
		minor m4 = new minor(null, 1, 50);
		m4.create(1);
		m4.intake(50);
		System.out.println("_____________________________________________");
		minor m5 = new minor(null, 3, 150);
		m5.create(3);
		m5.intake(150);

		System.out.println("_____________________________________________");
		System.out.println();
		System.out.println("The strength Of Different Schools: ");
		m3.strength();

	}

}
