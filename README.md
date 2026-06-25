Permament Magnet Synchronous Motor

```
Vd = - V ⋅ sin(σ)
Vq = V ⋅ cos(σ)
V = √ (Vd^2 + Vq^2)

σ = atan2(-Vd, Vq)

Id = I ⋅ cos(γ)
Iq = I ⋅ sin(γ)
I = √ (Id^2 + Iq^2)

γ = atan2(Iq, Id)

𝛙dstator = L ⋅ Id
𝛙qstator = L ⋅ Iq

Vd = - ω ⋅ 𝛙qstator
Vq = ω ⋅ ( 𝛙rotor + 𝛙dstator )

E = ω ⋅ 𝛙rotor

Id = ( Vq - E ) / ( ω ⋅ L )
Iq = - Vd / ( ω ⋅ L )

X = ω ⋅ L

cos(θ) = ( Vd ⋅ Id + Vq ⋅ Iq ) / ( √ ( ( Vd ^ 2 + Vq ^ 2 ) ⋅ ( Id ^ 2 + Iq ^ 2 ) ) )
sin(θ) = ( Vq ⋅ Id - Vd ⋅ Iq ) / ( √ ( ( Vd ^ 2 + Vq ^ 2 ) ⋅ ( Id ^ 2 + Iq ^ 2 ) ) )

S = √ ( ( Vd ^ 2 + Vq ^ 2 ) ⋅ ( Id ^ 2 + Iq ^ 2 ) )

P = Vd ⋅ Id + Vq ⋅ Iq
Q = Vq ⋅ Id - Vd ⋅ Iq
S = V ⋅ I

P = E ⋅ Iq
Q = E ⋅ Id + X ⋅ ( Id ^ 2 + Iq ^ 2 )

T = 𝛙rotor ⋅ Iq

For this motor MTPA condition reached under Id  = 0, 
and MTPV condition under Vq = 0
```

Synchronous Reluctance Motor

```
Vd = - V ⋅ sin(σ)
Vq = V ⋅ cos(σ)
V = √ (Vd^2 + Vq^2)

σ = atan2(-Vd, Vq)

Id = I ⋅ cos(γ)
Iq = I ⋅ sin(γ)
I = √ (Id^2 + Iq^2)

γ = atan2(Iq, Id)

𝛙d = Ld ⋅ Id
𝛙q = Lq ⋅ Iq

Vd = - ω ⋅ 𝛙q
Vq = ω ⋅ 𝛙d

Id = Vq / ( ω ⋅ Ld )
Iq = Vd / ( ω ⋅ Lq )

Xd = ω ⋅ Ld
Xq = ω ⋅ Lq

cos(θ) = ( Vd ⋅ Id + Vq ⋅ Iq ) / ( √ ( ( Vd ^ 2 + Vq ^ 2 ) ⋅ ( Id ^ 2 + Iq ^ 2 ) ) )
sin(θ) = ( Vq ⋅ Id - Vd ⋅ Iq ) / ( √ ( ( Vd ^ 2 + Vq ^ 2 ) ⋅ ( Id ^ 2 + Iq ^ 2 ) ) )

S = √ ( ( Vd ^ 2 + Vq ^ 2 ) ⋅ ( Id ^ 2 + Iq ^ 2 ) )

P = Vd ⋅ Id + Vq ⋅ Iq
Q = Vq ⋅ Id - Vd ⋅ Iq
S = V ⋅ I

T = (Ld - Lq) ⋅ Id ⋅ Iq

For modulating motor with saturation we shall add F(s), where F(s) is asinh(s) / s, 
and where:

s = √ ( ( Id / Idsat ) ^ 2 + ( Iq / Iqsat ) ^ 2 )

Thus getting: 

𝛙d = Ld ⋅ Id ⋅ F(s)
𝛙q = Lq ⋅ Iq ⋅ F(s)

For this motor MTPA condition, without saturation, reached under Id = Iq, 
and MTPV condition under | Vd | = Vq
```
