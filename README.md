import org.junit.Test;
import static org.junit.Assert.*;

public class StringTest {

    @Test
    public void lengthTest() {
    	
        assertEquals(0, "".length());
        
        assertEquals(1, "a".length());
        
        assertEquals(2, "ab".length());
        
        assertEquals(3, "abc".length());
    }

    @Test
    public void charAtTest() {
    	
        assertEquals('H', "Hello".charAt(0));
        
        assertEquals('e', "Hello".charAt(1));
        
        assertEquals('o', "Hello".charAt(4));
    }

    @Test
    public void subStringTest() {
    	
        assertEquals("How", "How are you?".substring(0, 3));
        
        assertEquals("are you?", "How are you?".substring(4));
        
        assertEquals("are", "How are you?".substring(4, 7));
    }

    @Test
    public void indexOfTest() {
    	
        assertEquals(5, "Some string".indexOf('s'));
        
        assertEquals(1, "Some string".indexOf('o'));
        
        assertEquals(0, "Some string".indexOf('S'));
    }
}
