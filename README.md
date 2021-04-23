
= SETUP

Requires docker installed

- `curl -s "https://get.sdkman.io" | bash && source "$HOME/.sdkman/bin/sdkman-init.sh"`
- `sdk install java 16.0.0.hs-adpt`
- `docker run -d --name sonar -p 9000:9000 --restart always sonarqube`
- Go http://localhost:9000 into admin console and disable forceuser authentication

= Checkout and build

- `git clone git@github.com:raffaeleragni-deliveryhero/codekata-template-javia.git && cd codekata-template-java`
- `./mwnw clean install sonar:sonar`
- `xdg-open http://localhost:9000`

