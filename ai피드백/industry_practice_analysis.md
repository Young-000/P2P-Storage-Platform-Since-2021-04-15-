# 실제 P2P 저장소 플랫폼 관행 분석

## **1. 주요 플랫폼들의 실제 Pricing Structure**

### **Storj (가장 성숙한 P2P 저장소 플랫폼)**

#### **사용자 요금 구조**
- **Storage Fee**: $4/TB/month (고정 월 요금)
- **Bandwidth Fee**: $7/TB for egress (다운로드 시)
- **Free Tier**: 25GB storage + 25GB bandwidth/month
- **구조**: **Hybrid Pricing과 매우 유사** (기본 저장 + 사용량 기반 bandwidth)

#### **Provider 보상 구조**  
- **Storage Payment**: $1.50/TB/month (실제 저장된 데이터 기준)
- **Bandwidth Payment**: $20/TB for egress (실제 제공한 bandwidth 기준)
- **특징**: **실제 사용량에 비례한 보상** (당신 모델과 일치)

### **Filecoin (블록체인 기반)**

#### **사용자 요금 구조**
- **Storage Deal**: 용량과 기간에 따른 협상 가격
- **Retrieval Fee**: 데이터 검색 시 별도 요금
- **Gas Fee**: 블록체인 트랜잭션 비용
- **구조**: **Two-part Tariff와 유사** (저장 + 검색 분리)

#### **Provider 보상 구조**
- **Block Rewards**: 네트워크 참여에 대한 FIL 토큰 보상
- **Storage Deal Revenue**: 클라이언트와 직접 협상한 수익
- **특징**: **용량 기반 + 성과 기반 혼합**

### **Sia (오픈소스 P2P 저장소)**

#### **사용자 요금 구조**
- **Storage Cost**: ~$1-2/TB/month (시장 경쟁 기반)
- **Bandwidth Cost**: 별도 요금 없음 (저장 비용에 포함)
- **구조**: **Subscription에 가까움** (포괄적 요금)

#### **Provider 보상 구조**
- **Contract-based**: 저장 계약 기반 수익
- **Proof-of-Storage**: 실제 저장 증명 시에만 보상
- **특징**: **계약 이행에 따른 보상**

---

## **2. 시뮬레이션 코드**
