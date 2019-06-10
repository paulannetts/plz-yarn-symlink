package(default_visibility = [])

subinclude("//:yarn")


create_symlink(name = "step1",
           srcs=["my_sub_dir/test1.txt"],
           outs=["my_out_dir"])


check_symlink(name = "step2",
           srcs=["my_sub_dir/test1.txt"],
           deps =[":step1"],
           outs=["ok.txt"])

