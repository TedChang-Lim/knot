# 모델 전략 최종 확정 (2026.06.19)

## 결정사항

**헤나(나) + 마스터님이 함께 테스트 후 확정**

### ✅ 확정: auxiliary vision → GLM-4.6V-Flash (z.ai, 무료)
- MiMo V2.5 → GLM-4.6V-Flash(z.ai)로 교체 완료
- 비용: $0 (완전 무료)
- 이미지 분석 품질: MiMo V2.5급, 상세하고 안정적
- 502 에러 없음 (Gemini 2.5 Flash와 달리 안정적)
- 엔드포인트: `https://api.z.ai/api/paas/v4/` (OpenAI 호환)
- API 키: z.ai(글로벌) Google 로그인 후 발급

### ❌ 기각: GLM-4.7-Flash → DeepSeek V4 Flash 대체 불가
- **Rate Limit** 걸림 (무료 모델의 한계)
- 응답 품질 DeepSeek V4 Flash보다 낮음 (30B MoE vs 236B MoE)
- 컨텍스트는 1M으로 넉넉하나 모델 자체 지능 부족
- 결론: 일상 대화는 DeepSeek V4 Flash 유지

### 최종 모델 아키텍처
| 구분 | 모델 | 비용 |
|:----|:----|:---:|
| 💬 일상 대화 | DeepSeek V4 Flash | $0.14/$0.28 |
| 🧠 복잡 추론 | DeepSeek V4 Pro | $0.435/$0.87 |
| 👁️ 이미지 분석 | GLM-4.6V-Flash | $0 (무료) 🆓 |

### z.ai(글로벌) 계정 정보
- 가입 방식: Google OAuth (nanal737@gmail.com)
- API 키명: "Hermes auxiliary vision"
- PAAS 엔드포인트: `https://api.z.ai/api/paas/v4/`
- Coding Plan: 구독 안 함 (유료라서)

### bigmodel.cn(중국) 검토 보류
- 2,000만 토큰 + 초대 2억 토큰 프로모션 존재 확인
- 단, 중국 전화번호 인증 + 실명 인증 필요
- GLM-5.2 등 프리미엄 모델이 필요해지면 그때 재검토
