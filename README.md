# P-SDK Detector

P-SDK Detector is a dependency detector for Payment SDK in Android. It extends LibScout, which is a light-weight and effective static analysis tool to detect third-party libraries in Android/Java apps. The detection is resilient against common bytecode obfuscation techniques such as identifier renaming or code-based obfuscations such as reflection-based API hiding or control-flow randomization. P-SDK detector profiles 965 versions of 49 popular payment SDK and detects their presence in Android apps. 


##  How to run:

java -jar LibScout.jar -o match -p profiles/Android -d output/ -a android.jar <i>path_to_app(s)</i>

Alternatively you can use batch_runner.py to run Libscout at scale

You can later use result_parser.py to output the results in a more readable format


## Scientific Publications

For technical details and large-scale evaluation results, please refer to the original publication:<br>
> - [Reliable Third-Party Library Detection in Android and its Security Applications](https://people.svv.lu/derr/publications/pdfs/derr_ccs16.pdf) (CCS'16)<br>


