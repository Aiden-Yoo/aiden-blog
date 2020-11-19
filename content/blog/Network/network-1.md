---
title: '[EVE-NG] 01. eve-ng 설치'
date: 2020-11-18 09:11:87
category: network
thumbnail: { thumbnailSrc }
draft: false
---

![](./images/network-1-01.png)

# 1. eve-ng?

eve-ng는 스위치를 가상화하여 LAB을 할 수 있는 시뮬레이터이다. 잘 알려진 시뮬레이터로 eve-ng, GNS3, Dynamips, VIRL가 있다.

# 2. 준비물

- 가상머신 (VMware, VirtualBox)
- FTP / SCP Client(WinSCP, FileZilla)
- 제품 가상 이미지

> eve-ng: v2.0.3-110 기준 작성

# 3. 다운로드

## eve-ng OVF 다운로드

![](./images/network-1-02.png)

`EVE-NG OVF`를 클릭하여 다운로드 후 압축 해제

## eve-ng Windows Client Side 다운로드

![](./images/network-1-03.png)

`Windows integration pack`을 클릭하여 다운로드

![](./images/network-1-04.png)

## VMware 다운로드

[Download](https://my.vmware.com/en/web/vmware/downloads/info/slug/desktop_end_user_computing/vmware_workstation_player/16_0)로 이동하여 `VMware workstation` 다운로드 및 설치

VirtualBox 등 다른 가상머신을 사용해도 되지만, 본 예시에서는 VMware를 사용한다.

## WinSCP 다운로드

[Download](https://winscp.net/eng/docs/guide_install)로 이동하여 `WinSCP` 다운로드 및 설치

스위치 이미지 등의 파일을 eve-ng로 전송하기 위해 FTP/SCP를 사용한다.
FileZilla 등 다른 FTP 클라이언트를 사용해도 되지만, 본 예시에서는 WinSCP를 사용한다.

# 4. 구성 절차

## VMware

1. File -> Open -> 다운받은 `EVE-COMM-VM.ovf` 선택

![](./images/network-1-05.png)

![](./images/network-1-06.png)

2. 가상 머신 경로와 파일명 지정

![](./images/network-1-07.png)

![](./images/network-1-08.png)

3. 가상머신 설정 변경

![](./images/network-1-09.png)

![](./images/network-1-10.png)

> `Virtualize Inter-x/EPT or AMD-V/RVI` 체크

![](./images/network-1-11.png)

> `NAT` 체크

4. 가상머신 실행 및 로그인

![](./images/network-1-12.png)

![](./images/network-1-13.png)

> `ID/PW(root/eve)` 입력

5. 기타 설정 적용

![](./images/network-1-14.gif)

6. 정상 로그인 확인

![](./images/network-1-15.png)

> 변경한 PW 입력

![](./images/network-1-16.png)

> `admin/eve` 입력하여 접속

## Windows Client

![](./images/network-1-17.png)

> EVE-NG `Windows Client` 설치
