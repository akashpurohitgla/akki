import java.util.regex.Matcher;
import java.util.regex.Pattern;

public class RegularExpressioin {
    public static void main(String[] args) {
        Pattern p=Pattern.compile("[A-Za-z0-9._]+@(gmail|hotmail|yahoo).com");
        Matcher m =p.matcher("amankumardagur7878@gmail.com");
        int c=0;
        while(m.find())
        {
            c++;
        }
        System.out.println(c);
    }
}
