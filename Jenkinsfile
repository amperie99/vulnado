pipeline {
    
    agent any
    stages {
        
        stage('build') {
            steps {
                sh 'mvn package'
                sh 'sl auth --no-diagnostic --org "467bc091-089e-48fc-a948-18c9786b1fc9" --token "eyJhbGciOiJSUzUxMiIsInR5cCI6IkpXVCJ9.eyJpYXQiOjE2MTUzMjQ5MDMsImlzcyI6IlNoaWZ0TGVmdCIsIm9yZ0lEIjoiNDY3YmMwOTEtMDg5ZS00OGZjLWE5NDgtMThjOTc4NmIxZmM5IiwidXNlcklEIjoiNzI0OGNhZjUtODk3Yi00NDFkLThjNWUtNDU4ZGNiMjUwNDdiIiwic2NvcGVzIjpbInNlYXRzOndyaXRlIiwiZXh0ZW5kZWQiLCJhcGk6djIiLCJ1cGxvYWRzOndyaXRlIiwibG9nOndyaXRlIiwicGlwZWxpbmVzdGF0dXM6cmVhZCIsIm1ldHJpY3M6d3JpdGUiLCJwb2xpY2llczpjdXN0b21lciJdfQ.OyKgdXlbbyrsWbjTl_3QWp2flgq2j-Z71h_o91Kq7cJjQAAlFBlIJfb74PNyf6Zmjof9mWRG4Z0B9V9B_IYet_9ggZ3VGB-CAS3VKbriKQxz_4SIxwr2Qqd8bNsEocgTzB7a_c2l-zejff4xtTPobdEKBg0KQWFIMYzdAPI1mJe5YleDJVvsEo3K3kEqhQ2E8lsEGlvkUMTLpnA8Bv-8ihfmoqKSofq7H343ooLXBYpFk6LeFdB-jKLe-6KKBwbFbyyX_H3qDevXYJZujulEccSRcewvK_IF-fLNLDqdEiXbNjzPCTQRGkS9dfJ_gecH-n5_FPRTibEiIghehJHvQQ"'
                sh 'sl analyze --app vulnado --java target/vulnado-0.0.1-SNAPSHOT.jar'
            }
        }
    }
}
