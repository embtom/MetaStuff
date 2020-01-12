set(SOURCE "main.cpp"
           "StringCast.cpp"
)

set(HEADERS "JsonCast.h"
            "JsonCast.inl"
            "StringCast.h"
)

add_executable(optinal_variant_json ${SOURCE} ${HEADERS})
target_link_libraries(optinal_variant_json 
    nlohmann_json 
    MetaStuff
)
