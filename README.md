# FaceRec
A Face Recognition tool, under unconstrained environments &amp; in real-time and derived from <a href= "https://github.com/deepinsight/insightface">insightface</a>.
<h1> Installation </h1>
installation requirement:

    pip install -r requirements.txt
<h2> Inference </h2>    
For face detection, run the following command:

     python inference_detection.py --input input/MBS.jpg    
In order to conduct "face identification" process, "feature extraction" and make the consequent comparison, please execute the following command:

    python inference_identification.py --input1 input/MBS0.jpg --input2 input/MBS1.jpg

Face Recognition will be done after executing:

    python inference_recognition.py --input ./io/input/MBS2.jpg --update

By default, the output result will be stored at `./output` repository.
