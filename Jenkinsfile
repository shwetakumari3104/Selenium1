pipeline{
agent any

tools{
maven 'Maven'
}
stages{
stage('Checkout')
{
steps
{
git branch:'master', url:"https://www.github.com/Shweta311204/Selenium1.git"
}}
stage('Build')
{
steps{
sh 'mvn clean package'
}}
stage('Test')
{
steps
{
sh 'mvn test'
}}
stage('Run')
{
steps
{
sh 'mvn exec:java -Dexec.mainClass="com.example.App"'
}}}
}
