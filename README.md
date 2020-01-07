# AmazonRecognition
- Set up access key, secret key and region (example us-east-1) in app.php, inside the function faceRecognition().

$client = new Aws\Rekognition\RekognitionClient([
         'version' => 'latest',
         'region' => 'your region',
         'credentials' =>[
            'key' => 'your key',
            'secret' => 'your key'
         ]
      ]);
 
 
 - Set up your own target image inside img folder. Name it target.png
