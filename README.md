# PlutoPkgTestRegistry
 
A small package registry used to test [Pluto's built-in package manager](https://github.com/fonsp/Pluto.jl/pull/844). 

Generated using [LocalRegistry.jl](https://github.com/GunnarFarneback/LocalRegistry.jl), which you should also use to modify this registry.

## Test packages
Registered are:
- [PlutoPkgTestA.jl](https://github.com/JuliaPluto/PlutoPkgTestA.jl)
- [PlutoPkgTestB.jl](https://github.com/JuliaPluto/PlutoPkgTestB.jl)
- [PlutoPkgTestC.jl](https://github.com/JuliaPluto/PlutoPkgTestC.jl)
- [PlutoPkgTestD.jl](https://github.com/JuliaPluto/PlutoPkgTestD.jl)
- [PlutoPkgTestE.jl](https://github.com/JuliaPluto/PlutoPkgTestE.jl)
- [PlutoPkgTestErrorA.jl](https://github.com/JuliaPluto/PlutoPkgTestErrorA.jl) (will `error()` when you import it)

With compatibilities:

- `A` has versions `0.1`, `0.2`, `0.3`: https://github.com/JuliaPluto/PlutoPkgTestRegistry/blob/main/P/PlutoPkgTestA/Versions.toml
- `B` depends on `A`@`0.2,0.3`: https://github.com/JuliaPluto/PlutoPkgTestRegistry/blob/main/P/PlutoPkgTestB/Compat.toml
- `C` depends on `A`@`0.2`: https://github.com/JuliaPluto/PlutoPkgTestRegistry/blob/main/P/PlutoPkgTestC/Compat.toml
- `D` and `E` have no compat bounds yet
