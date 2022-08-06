# APP1 PHP Laravel Project Deploy in Kubernetes Cluster

For the laravel application here, I use latest composer and PHP 7.4 image. Firstly I've installed composer in my host machine and generate a project using composer. 
Then I got the souce code and modified as per my need. To get the mentioed output I've created route in web.php file under routes direcroty like below.

Route::get('/app1', function () {
    return view('app1');
});

And create a app1.blad.php file as followkng in resources/views location

<!DOCTYPE html>
<html lang="{{ str_replace('_', '-', app()->getLocale()) }}">
<h3> Hello I am App 1 </h3>
</html>

Here, first portion of the blad.php file called app1 should match with route /app1. 
# Build image and push: 
When I done then create Dockerfile and docker compose file to build the image. 



