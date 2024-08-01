<p align="center"><a href="https://api.toedoe.hakudan.online/">Toedoe Api</a></p>

## Route list

- POST            api/auth/login .......................................... Api\Auth\LoginController
- POST            api/auth/logout ........................................ Api\Auth\LogoutController
- POST            api/auth/register .................................... Api\Auth\RegisterController
- GET|HEAD        api/user ......................................................................... 
- GET|HEAD        api/v1/tasks ........................... tasks.index › Api\V1\TaskController@index
- POST            api/v1/tasks ........................... tasks.store › Api\V1\TaskController@store
- GET|HEAD        api/v1/tasks/{task} ...................... tasks.show › Api\V1\TaskController@show
- PUT|PATCH       api/v1/tasks/{task} .................. tasks.update › Api\V1\TaskController@update
- DELETE          api/v1/tasks/{task} ................ tasks.destroy › Api\V1\TaskController@destroy
- PATCH           api/v1/tasks/{task}/complete ....................... Api\V1\CompleteTaskController
- GET|HEAD        api/v2/summaries ........................................ Api\V2\SummaryController
- GET|HEAD        api/v2/tasks ........................... tasks.index › Api\V2\TaskController@index
- POST            api/v2/tasks ........................... tasks.store › Api\V2\TaskController@store
- GET|HEAD        api/v2/tasks/{task} ...................... tasks.show › Api\V2\TaskController@show
- PUT|PATCH       api/v2/tasks/{task} .................. tasks.update › Api\V2\TaskController@update
- DELETE          api/v2/tasks/{task} ................ tasks.destroy › Api\V2\TaskController@destroy
- PATCH           api/v2/tasks/{task}/complete ....................... Api\V2\CompleteTaskController
- POST            auth/login .................................................. Auth\LoginController
- POST            auth/logout ................................................ Auth\LogoutController
- POST            auth/register ............................................ Auth\RegisterController
- GET|HEAD        sanctum/csrf-cookie sanctum.csrf-cookie › Laravel\Sanctum › CsrfCookieController@show
- GET|HEAD        up ............................................................................... 

## Main functions
- login
- logout
- register
- CRUD tasks (each user can only interacts with his/her own tasks)
- complete tasks (change status)
- view summaries by time period

## Deployment
Deployed with Nginx on Ubuntu using Digitalocean
