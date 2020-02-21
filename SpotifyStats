import java.io.*; 
import java.util.*; 

//Rivka Salem 

public class MusicStats {
//	private static final String[] String = null;

	public static void main(String[]args) throws IOException{
		//Read in file using bufferreader
		FileReader file = new FileReader("C:\\Users\\rivka\\Downloads\\SpotifyStats.csv"); 

		BufferedReader br = new BufferedReader(file); 
		
		ArrayList<String> positions = new ArrayList<String>();
		ArrayList<String> tracks = new ArrayList<String>();
		ArrayList<String> artists = new ArrayList<String>();
		ArrayList<String> streams = new ArrayList<String>();
		ArrayList<String> links = new ArrayList<String>(); 
		String line;
		
		while ((line = br.readLine()) != null) {	
		String []info = line.split(","); 
			
			String pos = info[0]; 
			positions.add(pos); 
			
			String tr = info[1]; 
			tracks.add(tr); 
			
			String art = info[2]; 
			artists.add(art);
			
			String str = info[3]; 
			streams.add(str);
			
			String lnk = info[4]; 
			links.add(lnk); 
			
		}
	br.close();  
	
	//Lets sort the arraylist to put artists in alphabetical order, used import from java.util
   System.out.println("\nBefore Sorting Artists List: " + artists); 
	Collections.sort(artists);
	System.out.println("\nSorted Artists List: "+ artists); 
	
	//Remove duplicates from artists arraylist using LinkedHashSet
	  Set<String> removed = new LinkedHashSet<String>(artists); 
	  System.out.println("\nList of artists duplicates removed: " + removed); 
	  
	  System.out.println("\nMost streamed Artist: "+ artists.get(0));
	  System.out.println("");
	  System.out.println("Artists names in alphabetical order: " + removed);

	    FileWriter fileWriter = new FileWriter("C:\\Users\\rivka\\eclipse-workspace\\Rivka 2019\\output.txt");
	    PrintWriter printWriter = new PrintWriter(fileWriter);
	    printWriter.println("Most streamed Artist: "+ artists.get(0)); 
	    printWriter.println("Artists names in alphabetical order: " + removed);
	    printWriter.close();
	  
	}
}











