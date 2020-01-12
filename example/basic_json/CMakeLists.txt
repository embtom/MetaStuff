set(SOURCE "main.cpp"
            "StringCast.cpp"
)

set(HEADERS "JsonCast.h"
            "JsonCast.inl"
            "MovieInfo.h"
            "Person.h"
            "StringCast.h"
)

add_executable(basic_json ${SOURCE} ${HEADERS})
target_link_libraries(basic_json 
    nlohmann_json 
    MetaStuff
)
