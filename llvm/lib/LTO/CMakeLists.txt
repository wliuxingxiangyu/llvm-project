add_llvm_component_library(LLVMLTO
  Caching.cpp
  LTO.cpp
  LTOBackend.cpp
  LTOModule.cpp
  LTOCodeGenerator.cpp
  SummaryBasedOptimizations.cpp
  UpdateCompilerUsed.cpp
  ThinLTOCodeGenerator.cpp

  ADDITIONAL_HEADER_DIRS
  ${LLVM_MAIN_INCLUDE_DIR}/llvm/LTO

  ENABLE_PLUGINS

  DEPENDS
  intrinsics_gen
  llvm_vcsrevision_h
)
