# ---------------------------------------------------------
cmake_minimum_required(VERSION 2.6)

project(LibAnimKit)
SET(${PROJECT_NAME} 1.0)

set(ANIMKIT_SRC 
	akAnimatedObject.cpp
	akAnimationChannel.cpp
	akAnimationClip.cpp
	akAnimationCurve.cpp
	akAnimationEngine.cpp
	akAnimationPlayer.cpp
	akAnimationPlayerSet.cpp
	akBufferInfo.cpp
	akDualQuat.cpp
	akGeometryDeformer.cpp
	akMathUtils.cpp
	akMesh.cpp
	akMorphTarget.cpp
	akPose.cpp
	akPoseBlender.cpp
	akSkeleton.cpp
	akSkeletonPose.cpp
	akTransitionBlender.cpp
	akVertexGroup.cpp
	
	btAlignedAllocator.cpp
)

set(ANIMKIT_HDR
	akAnimatedObject.h
	akAnimationChannel.h
	akAnimationClip.h
	akAnimationCurve.h
	akAnimationEngine.h
	akAnimationPlayer.h
	akAnimationPlayerSet.h
	akBufferInfo.h
	akColor.h
	akCommon.h
	akDualQuat.h
	akEuler.h
	akGeometryDeformer.h
	akMathUtils.h
	akMesh.h
	akMorphTarget.h
	akPose.h
	akPoseBlender.h
	akSkeleton.h
	akSkeletonPose.h
	akTransformState.h
	akTransitionBlender.h
	akVertexGroup.h
	
	btAlignedAllocator.h
	btAlignedObjectArray.h
)

include_directories(${GAMEKIT_UTILS_PATH} ${ANIMKIT_VECTORMATH_PATH})

add_library(${PROJECT_NAME} ${ANIMKIT_HDR} ${ANIMKIT_SRC})

