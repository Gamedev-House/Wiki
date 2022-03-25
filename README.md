# Полезные материалы
- [Кодстайл, которого нужно придерживаться](https://github.com/raywenderlich/c-sharp-style-guide)
- [Документация Git](https://git-scm.com/)
- [Документация Unity](https://docs.unity3d.com/Manual/index.html)
- [Документация New Input System](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.0/manual/)
- [Документация ProBuilder](https://docs.unity3d.com/Packages/com.unity.probuilder@5.0/manual)
- [Моя старая группа в ТГ с кучей полезного](https://t.me/road_to_gamedev)
Ассеты, которые мы используем
- [Unity Atoms](https://unity-atoms.github.io/unity-atoms/)
- Каналы с VR тематикой: [ValemVR](https://www.youtube.com/c/ValemVR), [JustinPBarnett](https://www.youtube.com/c/JustinPBarnett), [VRwithAndrew](https://www.youtube.com/c/VRwithAndrew), [DilmerV](https://www.youtube.com/c/DilmerV)

# Типовые ошибки
- Отдавать некомпилирующийся код в ветке. В частности из-за того, что логический код (использующий `UnityEngine`) перемешан с кодом эдитора (использующим `UnityEditor`). Куски кода, которые используют эдитор (часто методы под аттрибутом `ContextMenu` или `OnValidate`) нужно оборачивать в `#if UNITY_EDITOR`, либо класть отдельно в папку `Editor` (см. https://docs.unity3d.com/Manual/SpecialFolders.html)
