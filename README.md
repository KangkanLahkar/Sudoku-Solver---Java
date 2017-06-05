# Sudoku-Solver---Java
This is a java sudoku solver. One can use this either by entering values in 9*9 grid or passing an array manually

How to use it?
1. Extract the files in eclipse.
2. Run the class UI.java.
3. A pop screnn containing 9*9 grid would appear.
4. Click on any grid. Another pop up will appear.
5. In the pop up one can enter values of the grid.
6. After you finished entering the values you can click on "Solve" option in the pop up and then "OK".
7. If you need to clear the grid click "Clear all" then "OK"

Also there is other option to manually create a 9*9 array and pass it to the solver class
Suppose this is your sudoku grid. (Blank spaces are initialised with 0)
int [][]arr1 =  {{0,0,0,0,0,0,0,0,0},
				         {0,0,0,0,0,3,0,8,5},
				         {0,0,1,0,2,0,0,0,0},
				         {0,0,0,5,0,7,0,0,0},
				         {0,0,4,0,0,0,1,0,0},
				         {0,9,0,0,0,0,0,0,0},
				         {5,0,0,0,0,0,0,7,3},
				         {0,0,2,0,1,0,0,0,0},
				         {0,0,0,0,4,0,0,0,9}};
                 
 Create a object to Solver class
     Solver sv = new Solver(arr1);
     if(sv.solve()){
			System.out.println(Arrays.deepToString(arr1).replace("],", "],\n"));
		  }else{
			System.out.println("Solution doesn't exist");
		 }
 
 Or alternatively you can
    Solver sv1 = new Solver();
		if(sv1.solve(arr2)){
			System.out.println(Arrays.deepToString(arr2).replace("],", "],\n"));
		}else{
			System.out.println("Solution doesn't exist");
		}
                 
