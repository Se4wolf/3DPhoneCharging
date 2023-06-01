# 3D модель зардяки телефона

## Программы
- **Blender 3.5.1**
## Актуальность
В наше время навык создания трёхмерной визуализации является очень важным для демонстрации продукта или использования в AR- и VR- приложениях.
<p align="center">
<img src="Examples/Blender.png" alt=""><br>
<i>Программа для создания 3D моделей</i>
</p>  


## Runtime Manager
The auto rigger contains a lot of helper joints, these helper joints are not going to be driven by the Unity's Mecanim system. The runtime manager script allows you to apply the .skeletonPreset file exported in Maya to the skeleton in Unity. It will apply scripts to the helper joints and set the correct settings coming from Maya meaning the deformation will be identical between the two applications. Once this process is done the helper joints are driven by joints that are controlled by the Mecanim system.

<p align="center">
<img src="Examples/runtimeManagerInspector.png" alt="Runtime Manager Inspector"><br>
<i>Runtime Manager Inspector</i>
</p>


## Runtime Helper
The runtime helper setup contains 2 different scripts. The helper joints are used to preserve volume in areas like the hips, knee, wrist, elbow etc. The helper translate script will preserve volume by translating the joint based on rotational values and the helper aim joint will preserve volume aiming its joint towards a target. The aim joint is a child of the translate joint.

<p align="center">
<img src="Examples/runtimeHelper.gif" alt="Runtime Helper Example"><br>
<i>Runtime Helper Example</i>
</p>

<p align="center">
<img src="Examples/runtimeHelperTranslateInspector.png" alt="Runtime Helper Translate Inspector"><br>
<i>Runtime Helper Translate Inspector</i>
</p>

<p align="center">
<img src="Examples/runtimeHelperAimInspector.png" alt="Runtime Helper Aim Inspector"><br>
<i>Runtime Helper Aim Inspector</i>
</p>

## Runtime Twister
The runtime twister can split the twist value of a parent joint and only apply a fraction of that to the helper joint. This will help prevent the candy wrapper effect.

<p align="center">
<img src="Examples/runtimeTwister.gif" alt="Runtime Twister Example"><br>
<i>Runtime Twister Example</i>
</p>

<p align="center">
<img src="Examples/runtimeTwisterInspector.png" alt="Runtime Twister Inspector"><br>
<i>Runtime Twister Inspector</i>
</p>

## Runtime Muscle
The runtime muscle is the more complex of the runtime joints. It mimics the behaviour of a muscle, it has a origin and an insertion point driven by parent joints. This script also features an option that is not available in Maya, it is possible to make the joint dynamic. The dynamics will add a natural jiggle to the joint which boosts realism.

<p align="center">
<img src="Examples/runtimeMuscle.gif" alt="Runtime Muscle Example"><br>
<i>Runtime Muscle Example</i>
</p>

<p align="center">
<img src="Examples/runtimeMuscleInspector.png" alt="Runtime Muscle Inspector"><br>
<i>Runtime Muscle Inspector</i>
</p>

### Credits
* Modelling Topology: <a href="http://www.makehuman.org">Make Human</a>
* Modelling: <a href="https://www.artstation.com/mfalzon"><strong>Michael Falzon</strong></a>
* Animation: <a href="https://assetstore.unity.com/packages/3d/animations/everyday-motion-pack-free-115067">Everyday Motion Pack Free</a>
