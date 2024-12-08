# Arraylist
import java.util.ArrayList;
import java.util.Collections;
import java.util.Iterator;

public class Arraylist {
    public Arraylist() {
    }

    public static void main(String[] args) {
        ArrayList<String> arrayList = new ArrayList();
        arrayList.add("sakshat");
        arrayList.add("Pranay");
        arrayList.add("Vishist");
        arrayList.add("Madhur");
        System.out.println("The arraylist before sorted:");
        Iterator var2 = arrayList.iterator();

        String str;
        while(var2.hasNext()) {
            str = (String)var2.next();
            System.out.println(str);
        }

        Collections.sort(arrayList, Collections.reverseOrder());
        System.out.println("The arraylist in descending order;");
        var2 = arrayList.iterator();

        while(var2.hasNext()) {
            str = (String)var2.next();
            System.out.println(str);
        }

    }
}
