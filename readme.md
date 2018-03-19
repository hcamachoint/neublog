<h1>Laravel Blog Project</h1>

<p>Simple blog developed on laravel framework</p>

<h2>Twitter</h2>
<p>https://apps.twitter.com/</p>

<h2>Facebook</h2>
<p>https://developers.facebook.com/apps/</p>
<p>#Deshabilitar: Usar modo estricto para URI de redireccionamiento</p>

<h2>General</h2>
<p>URI de redirección de OAuth válidos: http://localhost:8000/auth/facebook/callback</p>

<p>Heroku Database</p>

$url = parse_url(getenv("DATABASE_URL"));
$host = $url["host"];
$username = $url["user"];
$password = $url["pass"];
$database = substr($url["path"], 1);

'pgsql' => [
  'driver'   => 'pgsql',
  'host'     => $host,
  'database' => $database,
  'username' => $username,
  'password' => $password,
  'charset'  => 'utf8',
  'prefix'   => '',
  'schema'   => 'public',
  ],
