# AmazonRecognition
- Set up access key and secret key in app.php, inside the function faceRecognition(). 
$client = new Aws\Rekognition\RekognitionClient([
         'version' => 'latest',
         'region' => 'us-east-1',
         'credentials' =>[
            'key' => 'your key',
            'secret' => 'your key'
         ]
      ]);
      
 - Set up your own target image inside img folder. Name it target.png
