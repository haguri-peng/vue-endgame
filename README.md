# vue-endgame study
vue-endgame (feat. joshua1988)

# mongoDB connect parameter
mongoose.connect(
	// 'mongodb+srv://test:1234@cluster0-ypgh5.mongodb.net/test?retryWrites=true&w=majority',
	'mongodb+srv://test:1234@cluster0.ukngq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority',
	{
		useNewUrlParser: true,
		useUnifiedTopology: true,
	}
);

# Node version issue
nvm 으로 버전을 10.16.3 으로 지정하면, 버전 문제로 @vue/cli 를 사용할 수 없다.
그렇다고 버전을 최신으로 하면 vue-til-server 가 동작하지 않는데..
서버에서 사용하는 'bcrypt' 버전(작성 당시 버전 5.0.1)을 최신으로 업데이트 해주면 정상적으로 작동한다.
npm install bcrypt@latest
