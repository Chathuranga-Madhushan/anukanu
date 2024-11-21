# anukanu
//labsheet 2

/home/ICt/tarballs/ns-allinone-3.43/ns-3.43/scratch
./ns3 run scratch/first.cc



    //Ascii trace helper
    AsciiTraceHelper ascii;
    pointToPoint.EnableAsciiAll(ascii.CreateFileStream("512.tr"));
  
ls
cd t
cd tracemetrics-1.4.0
java -jar tracemetrics.jar


#include "ns3/netanim-module.h"

    //net animation
    AnimationInterface anim("p2p.xml");

/home/ICt/tarballs/ns-allinone-3.43/netanim-3.109
./NetAnim
open p2p.xml from ns3


//labsheet 5
gnuplot
plot sin(x)

using tab key enter the table values 
save >> mydata.txt desktop

set terminal pdf 
set output "gnuplot.pdf"
set xlabel "No of Speed"
set ylabel "Speed"
pot "mydata.txt"using 1:2 with impluse title "speed Km/h" lw 2, "mydata.txt" using 1:3 with linespoint title "Age" lw 2


save >> mygnucode.plt desktop
open terminal on desktop
gnuplot my
gnuplot mygnucode.plt

under the mygnucode.plt
>>
set terminal png size 600,400
set output "gnuplot.png"
set title "Driver's salary"
set xlabel "Number of Days"
set ylabel "Driver salary"
plot "mydata.txt" using 1:4 with linespoints title "Salary in Rs " lw 2,2000 title "Minimum salary " lw 2

>>run again
gnuplot mygnucode.plt



gnuplot mygnucode2.plt


set terminal pdf
set output 'AQL_Histogram.pdf'

set title "City AQI_Comparison"
set boxwidth 0.4
set style fill solid

# set labels and grid
set xlabel "City"
set ylabel "Air Quality Index (AQI)"
set grid ytics

#set xtics to use the first column from the data file
set xtics rotate by -45 font ",8" nomirror

# Define data format and plot style
plot 'mydata.data' using 2:xtic(1) title "AQI Last Month" with boxes lc rgb "blue", \
	'' using 3:xtic(1) title "AQI Current Month" with boxes lc rgb "red"

