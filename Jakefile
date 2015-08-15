desc('Make the package available.');
task('default', function () {
	jake.mkdirP('js');
	jake.mkdirP('css');
	jake.mkdirP('font');
	jake.exec([
		'cp -R bower_components/jquery/dist/* js/',
		'cp -R bower_components/materialize/dist/* ./'
	]);
});
desc('Clean up the directory.');
task('clean', function () {
	jake.rmRf('js');
	jake.rmRf('css');
	jake.rmRf('font');
});
desc('Run local demo.');
task('demo', function () {
	jake.exec('live-server --port=3001', { interactive: true });
});