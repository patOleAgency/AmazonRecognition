# AmazonRecognition

DESCRIPTION

This code uses Amazon Recognition to recognize a face in a group photo (target photo). 

Index.php shows the target photo and every certain seconds it cheks if a photo has been uploaded. In that case, it shows the uploaded photo on the right side and a red square in the target photo if that person has been recognised. By default, the square is at position top-left (it will stay there if the recognition result is below "SimilarityThreshold" value (set to 70% but can be changed in app.php). 

Upload.php is to upload the photo (it's set for mobile upload). 

SET-UP

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
