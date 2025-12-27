---
title: "MathJax 수식 렌더링 테스트"
date: 2025-12-27
categories: [notes]
tags: [mathjax, latex, test]
visibility: private
---

이 글은 **LaTeX 수식 렌더링 테스트용**이다.

---

## 1. 인라인 수식
에너지-질량 등가식은 $E = mc^2$ 이다.

회귀 문제에서 잔차는 $e_i = y_i - \hat{y}_i$ 로 정의한다.

---

## 2. 블록 수식
평균제곱오차(MSE):

$$
\mathrm{MSE}
= \frac{1}{n}\sum_{i=1}^{n}(y_i - \hat{y}_i)^2
$$

RMSE:

$$
\mathrm{RMSE}
= \sqrt{\frac{1}{n}\sum_{i=1}^{n}(y_i - \hat{y}_i)^2}
$$

---

## 3. 벡터 / 행렬
선형회귀:

$$
\mathbf{y} = \mathbf{X}\boldsymbol{\beta} + \boldsymbol{\epsilon}
$$

정규방정식:

$$
\hat{\boldsymbol{\beta}}
= (\mathbf{X}^\top \mathbf{X})^{-1}\mathbf{X}^\top \mathbf{y}
$$

---

## 4. 확률 / 통계
정규분포:

$$
p(x \mid \mu, \sigma^2)
= \frac{1}{\sqrt{2\pi\sigma^2}}
\exp\left(-\frac{(x-\mu)^2}{2\sigma^2}\right)
$$

---

## 5. 코드 블록 (수식 렌더링 안 되어야 정상)
```python
def mse(y, y_hat):
    return ((y - y_hat) ** 2).mean()
```

---

## 6. 혼합 예시

손실함수는

$$
\mathcal{L}(\theta)
= \sum_{i=1}^{N} \ell\big(y_i, f_\theta(x_i)\big)
$$

이며, $\nabla_\theta \mathcal{L}$ 를 통해 최적화한다.

---