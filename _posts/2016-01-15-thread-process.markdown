---
layout: post
title:  "쓰레드와 프로세스를 설명하시오"
date:   2016-01-15 16:35:57 +0900
categories: jekyll update
---
쓰레드와 프로세스는 엄연히 다릅니다.
프로세스는 쉽게 말해서 하나의 작업 단위라고 할 수 있습니다.
그래서 멀티 프로세스로 작업을 한다면 서로 사용하는 메모리와 자원이 다르기에 자바에서 멀티 쓰레드 방식으로 프로그래밍을 합니다.
한 프로세스 내에 여러 쓰레드가 존재할수 있고 해당 쓰레드들은 자신을 포함한 프로세스의 자원을 공유합니다.
그래서 멀티 쓰레드 프로그래밍을 사용했을때 하드웨어의 성능에 따라서 단일 프로세스 내에서도
월등한 작업속도를 낼 수 있습니다.
단 쓰레드 하나하나를 직접 조작할 수 없기에 쓰레드들이 데이터를 물고 죽어버리던지 했을때
데이터의 유실에 주의하여하하고 각각 쓰레드들이 언제 데이터를 가지고 올지 속도 면에서도 확신을 할 수 없기에
이런 부분에서 주의를 요합니다.
자세한 사항은 예제를 만들어보시고 위의 synchronized 와 함께 사용해보시는것도 좋을듯 합니다.