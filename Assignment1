/**
 * 
 */
package LinkedList_A1;

import static org.junit.jupiter.api.Assertions.*;

import org.junit.jupiter.api.Test;

/**
 * @author jeroen
 *
 */
class testJUnit {

	
	@Test
	void test() {
		
		LinkedListImpl L = new LinkedListImpl();
		
		//List is empty, size should be one
		assertEquals(L.size(),0);
		
		//Removing non-existing items should result in false
		assertFalse(L.remove(0));
		assertFalse(L.remove(1));
		assertFalse(L.remove(2));
		assertFalse(L.remove(3));
		
		//Adding item to place that does not exist should be false
		assertFalse(L.insert(2.31, 1));
		
		//Adding item to empty list in spot 0 should be true
		assertTrue(L.insert(2.31, 0));
		
		//Try to retrieve that newly entered item
		assertEquals(L.get(0),2.31);
		
		//Try to put another item in 0
		assertTrue(L.insert(4.31, 0));
		
		//Item in 0 should now be 4.31, item in 1 should be 2.31
		assertEquals(L.get(0),4.31);
		assertEquals(L.get(1),2.31);
		
		//Try to add item to 3 should be false, because 2 does not exist
		assertFalse(L.insert(3.31, 3));
		
		//Try to add item to 2 should be true
		assertTrue(L.insert(3.31, 2));
		
		//Try to add item to 2 again should be true again
		assertTrue(L.insert(5.31, 2));
		
		//Size of list should be 4 by now
		assertEquals(L.size(), 4);
		
		//Index 0, 1, 2, 3 exist. True to retrieve those
		assertEquals(L.get(0),4.31);
		assertEquals(L.get(1),2.31);
		assertEquals(L.get(2),5.31);
		assertEquals(L.get(3),3.31);
		
		//Try to remove item at -1 should be false
		assertFalse(L.remove(-1));
		
		//Try to remove item at 0 should be true
		assertTrue(L.remove(0));
		
		//Size of list should be 3 by now
		assertEquals(L.size(), 3);
		
		//Try to remove item at 3 should be false
		assertFalse(L.remove(3));
		
		//Size of list should be 2 by now
		assertEquals(L.size(), 3);
		
	}

}
