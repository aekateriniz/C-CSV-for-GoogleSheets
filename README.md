# C-CSV-for-GoogleSheets

//Create CSV file for Google Sheets C++
//This is NOT for Excel




#include <iostream>
#include <fstream>
using namespace std;

int main() {
  // Create and open a text file
  ofstream MyFile("Project_Aekaterini.csv");


// Write to the file
  
MyFile<<"product_id,	product_category,	sku, upc,	warehouse_location, qty " <<endl;
MyFile<<"101,	mascara, A113M1, 3445-113-545,	Markham,	430" <<endl;
MyFile<<"102, mascara,	A212M2,	3445-212-454,	Markham, 120"<<endl;
MyFile<<"103,	nailpolish,	A221NP2,	3445-221-435,	Markham,	450"<<endl;
MyFile<<"104,	nailpolish,	A332NP2,	3445-332-003,	Markham,	910"<<endl;
MyFile<<"105,	lipgloss,	A36LIPG, 	3445-336-347,	Markham,	650"<<endl;
MyFile<<"106,	lipgloss,	A49LIPG, 	3445-432-523,	Markham,	1000"<<endl;
MyFile<<"107,	tint foundation,	A434TNT,	3445-434-777, Markham,	1000"<<endl;
MyFile<<"108,	lipgloss,	A48LIPG, 	3445-442-223,	Markham,	550"<<endl;
MyFile<<"109,	lipgloss,	A45LIPG,	3445-442-756,	Markham,	580"<<endl;
MyFile<<"110,	nailpolish,	A443NP5,	3445-443-676,	Markham,	840"<<endl;


//Spreadsheet Calculations

MyFile<<"Calculations"<<endl;
MyFile<<"=SUM(""F2:F11"")"<<endl;  
MyFile<<"=MIN(""F2:F11"")"<<endl;
MyFile<<"=MAX(""F2:F11"")"<<endl;
MyFile<<"=AVERAGE(""F2:F11"")"<<endl;


  // Close the file
  MyFile.close();
}
