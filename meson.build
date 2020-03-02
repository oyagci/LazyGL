project('LazyGL', 'cpp')

add_global_arguments('-DGLM_ENABLE_EXPERIMENTAL', language : 'cpp')

srcs = [
  'sources/inputs/Keyboard.cpp',
  'sources/inputs/Mouse.cpp',
  'sources/inputs/Input.cpp',
  'sources/maths/maths.cpp',
  'sources/graphics/Shader.cpp',
  'sources/graphics/Display.cpp',
  'sources/graphics/textures/Framebuffer.cpp',
  'sources/graphics/Camera.cpp',
  'sources/graphics/Mesh.cpp',
  'sources/utils/fileutils.cpp',
]

incdirs = [
  'includes/',
  'sources/',
  'sources/',
  'sources/maths',
  'sources/graphics',
  'sources/graphics/textures',
  'sources/utils',
]

glew = dependency('glew', required: true)
glfw = dependency('glfw3', required: true)
gl = dependency('GL', required: true)

deps = [ glew, glfw, gl ]

shared_library('LazyGL', srcs, dependencies: deps, include_directories: incdirs)
