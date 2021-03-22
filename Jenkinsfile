buildDockerAndPublishImage('jenkins', [
    mainBranch: 'main', 
    registry: 'garethjevans/', 
    credentials: 'docker-credentials',
    automaticSemanticVersioning: true,
    gitCredentials: 'github-app-testserver',
    metadataFromSh: "cat Dockerfile | grep FROM | sed 's|FROM jenkins/jenkins:|+|' | sed 's|-lts-jdk11||'"
])  
