node() {
  properties([parameters([string(defaultValue: '', description: '', name: 'ip', trim: true)])])
  withEnv(["DUMMY_SERVER_URL=http://${params.ip}:8080"]) {
    sh 'python /dummy_server_tests.py -v'
  }
}
