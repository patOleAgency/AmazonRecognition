# AmazonRecognition
- Install Amazon SDK for PHP from this site https://docs.aws.amazon.com/sdk-for-php/v3/developer-guide/getting-started_installation.html. Save the files inside a folder name aws in the root directory.

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
