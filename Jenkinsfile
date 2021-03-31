buildDockerAndPublishImage('jenkins', [
    mainBranch: 'main', 
    registry: 'garethjevans/', 
    credentials: 'docker-credentials',
    automaticSemanticVersioning: true,
    nextVersionCommand: 'jx-release-version -next-version=semantic:strip-prerelease',
    gitCredentials: 'github-app-testserver',
    metadataFromSh: "cat Dockerfile | grep FROM | sed 's|FROM jenkins/jenkins:|-|' | sed 's|-lts-jdk11||'"
])  
