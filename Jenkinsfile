node {
  stage 'Checkout'
  checkout scm

  stage 'Environment'
  sh 'env'

  stage 'Hello World'
  echo 'Hello, World!'

  if (env.CHANGE_ID != null) {
    stage 'Merge Test'
    echo "CHANGE_ID: $env.CHANGE_ID"
  }
}
