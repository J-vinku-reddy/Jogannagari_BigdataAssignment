https://beam.apache.org/get-started/quickstart-java/

mvn archetype:generate `
  -D archetypeGroupId=org.apache.beam `
  -D archetypeArtifactId=beam-sdks-java-maven-archetypes-examples `
  -D archetypeVersion=2.42.0 `
  -D groupId=org.example `
  -D artifactId=word-count-beam `
  -D version="0.1" `
  -D package=org.apache.beam.examples `
  -D interactiveMode=false
   
cd .\word-count-beam

dir .\src\main\java\org\apache\beam\examples

In the word-count-beam directory, create a file called sample.txt. Add some text to the file. For this example

mvn compile exec:java -D exec.mainClass=org.apache.beam.examples.WordCount `
 -D exec.args="--inputFile=sample.txt --output=counts" -P direct-runner

ls counts*
   
more counts*

Output :

certain: 1
tell: 1
calumny: 1
ugly: 1
soldier: 1
vows: 1
bestow: 2
further: 1
patient: 1
alone: 1
who: 2
pangs: 1
variable: 1
pause: 1
keeps: 1
confession: 1
returns: 1
honest: 3
Madness: 1
fit: 1
both: 1
delay: 1
you: 29
seeing: 1
sinners: 1
behaved: 1
am: 2
your: 13
beck: 1
shocks: 1
say: 2
death: 2
Take: 1
Your: 2
As: 1
yourselves: 1
The: 15
observers: 1
Soft: 1
an: 1
d: 9
needs: 1
hold: 1
I: 32
did: 3
lack: 1
never: 1
With: 5
as: 10
confusion: 1
leave: 1
go: 4
crawling: 1
for: 10
-- More  --