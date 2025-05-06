add_llvm_library(ELDLayout LayoutInfo.cpp LDYAML.cpp TextLayoutInfo.cpp
                 YamlLayoutInfo.cpp)

target_link_libraries(
  ELDLayout
  ELDConfig
  ELDFragment
  ELDSupport
  ELDDiagnostics
  ELDTarget
  ELDSymbolResolver)
