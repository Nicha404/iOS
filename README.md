# iOS 
 
## Bundle identifier

**A bundle ID or bundle identifier** uniquely identifies an application in Apple's ecosystem. This means that no two applications can have the same bundle identifier. To avoid conflicts, Apple encourages developers to use reverse domain name notation for choosing an application's bundle identifier.

***

## ARC 

***

## Concurrency

동기 VS 비동기

동기 - 메인 쓰레드에서 다른 쓰레드에 작업을 보낼 시 다른 쓰레드에 할당된 작업이 끝나야 다시 메인 쓰레드로 돌아온다.

비동기 - 메인 쓰레드에서 다른 쓰레드에 작업을 보내고 그 작업이 끝나든 말든 다시 메인 쓰레드로 돌아온다. 주로 서버와의 통신 때문에 비동기라는 개념이 생겼다. 네트워크 상황에 따라 앱 안에 처리할 작업간에 속도가 달라질 수 있다. 그래서 네트워크는 대부분 비동기 처리이다.

Serial VS Concurrency

Serial - 메인에서 분산처리 시킨 작업을 다른 한개의 쓰레드에서만 작업 진행.(작업에 순서가 필요할때)

Concurrency - 메인에서 분산처리 시킨 작업을 다른 여러개의 쓰레드에서 동시에 처리한다.(각각 독립적이지마 유사한 작업일 때 ex) 인스타 피드)

그럼 비동기와 동시성의 차이는 뭘까? 동기와 비동기는 메인 쓰레드를 중심으로 하는 말이고 Serial과 Concurrency는 보내진 쓰레드를 뜻한다.

iOS는 GCD / operation을 통해 큐에다가 작업을 보내주기만 하면 자동으로 쓰레드 할당을 한다.


 
 
