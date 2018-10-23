# PhoneSensorMath
A repository of math-oriented projects that incorporate data from sensors
found in typical cell phones. The projects are all rendered in jupyter
notebooks that have markdown annotations. To use these, download the .ipynb
and associated .csv files to your computer. Load the .ipynb file into
jupyter, modify to suit your needs.

## GPS Fastest Mile Analysis
This notebook describes the collection and analysis of GPS data recorded
during an exercise run/walk/bike. The analysis allows one to determine the
fastest mile within the longer exercises course. The notebook is documented
so that other lengths (i.e. kilometer) can be considered. Such an analysis
might accompany an introductory calculus curriculum about time vs.
distance.

## Accelerometer Frequency Analysis
This notebook describes the collection and analysis of phone accelerometer
data recorded while the phone rested on a clothes washer during its spin
cycle. The rate of spin is determined by using the discrete Fourier
transform and identifying the dominant frequency of vibration in the
accelerometer data. This analysis might accompany an engineering math
course as it discusses the discrete Fourier transform.

## Physics Toolbox Sensor Suite
Tips about recording with the physics toolbox sensor suite. I use the app on a OnePlus 3T phone. 
A lot of phones, like mine, want to conserve battery power and aggressively try to put idle apps to sleep. This _may_ cause your recordings of various sensors either fail to start, or to shutdown prematurely. The behavior is highly dependent on the phone. Make sure you understand your phone quirks _before_ you go out on a long recording only to find that the recording stopped halfway through the effort. Here are a few things that I've learned about my own phone. My knowledge of iPhone behavior in this area is practically zero. (__Note:__ if you have tips you'd like to add to this list, please send them to me.)

1. Lots of Android phones have a battery optimization section in the settings. This provides an app-by-app listing of battery optimization. It's wise to disable all battery optimization on whatever app you're using to record sensors.

1. GPS recording, go to the GPS sensor page in the app, hit the record button, go into "advanced stats" wait until GPS lock, then recording is happening, sometimes, if lock is lost during the recording, the recording will stop without notice. Sample rate is about 1Hz.

1. Accelerometer recording seems to work just hitting the record button, note that it generates a lot of readings since the sample rate is around 200Hz (at least on my phone).

1. Multirecording, to collect, for example, GPS and accelerometer data simultaneously, go to the GPS page and start a recording there (see above), go to the accelerometer page and start a recording there, _then_ go to the Multirecord page, check the Linear Accelerometer and GPS boxes and start recording there. 

1. In general, most of the issues seem to center around getting the GPS to lock and _stay_ locked.