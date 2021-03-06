cmake_minimum_required(VERSION 3.14)
project(ft_json)

add_compile_options(-Wall -Wextra -Werror)

include_directories(. libft/include include)

add_library(ft STATIC
		libft/src/ft_astr_astr.c
		libft/src/ft_isprint.c
		libft/src/tview_init.c
		libft/src/ft_atolu_base.c
		libft/src/ft_cadd.c
		libft/src/ft_strdup.c
		libft/src/ft_strput.c
		libft/src/ft_lstdel.c
		libft/src/ft_atol_base.c
		libft/src/ft_memchr.c
		libft/src/ft_lstnew.c
		libft/src/ft_tpointer.c
		libft/src/ft_putnbr.c
		libft/src/ft_atou_base.c
		libft/src/ft_astr_len.c
		libft/src/ft_nsym.c
		libft/src/ft_strncat.c
		libft/src/ft_strncpy.c
		libft/src/ft_strlen.c
		libft/src/ft_putstr_fd.c
		libft/src/tview.c
		libft/src/ft_tpointer_keeper_attr.c
		libft/src/ft_bzero.c
		libft/src/ft_putendl.c
		libft/src/ft_isspace.c
		libft/src/ft_strnchri.c
		libft/src/ft_strequ.c
		libft/src/ft_memccpy.c
		libft/src/ft_bit_endian.c
		libft/src/ft_cpowl.c
		libft/src/ft_isupper.c
		libft/src/ft_isalpha.c
		libft/src/ft_putendl_fd.c
		libft/src/ft_memcpy.c
		libft/src/ft_tpointer_get.c
		libft/src/ft_strnlen.c
		libft/src/twin.c
		libft/src/ft_strtrim.c
		libft/src/ft_memmove.c
		libft/src/ft_astr_del.c
		libft/src/ft_strnequ.c
		libft/src/ft_tpointer_keeper_get.c
		libft/src/ft_itoa.c
		libft/src/get_next_line.c
		libft/src/ft_lstiter.c
		libft/src/ft_tpointer_keeper.c
		libft/src/ft_cabsl.c
		libft/src/ft_cdiv.c
		libft/src/ft_tolower.c
		libft/src/ft_strndup.c
		libft/src/ft_strmapi.c
		libft/src/ft_ishex.c
		libft/src/ft_strsub.c
		libft/src/ft_memalloc.c
		libft/src/ft_putchar.c
		libft/src/ft_putnbr_fd.c
		libft/src/ft_write_free.c
		libft/src/ft_csub.c
		libft/src/ft_strcat.c
		libft/src/ft_strlcat.c
		libft/src/ft_astr_new.c
		libft/src/ft_strncmp.c
		libft/src/ft_strlenc.c
		libft/src/ft_strnew.c
		libft/src/ft_memcmp.c
		libft/src/ft_striteri.c
		libft/src/ft_bit_mask.c
		libft/src/ft_lstmap.c
		libft/src/ft_uintlen.c
		libft/src/ft_atoll_base.c
		libft/src/ft_striter.c
		libft/src/ft_putchar_fd.c
		libft/src/ft_strsplit.c
		libft/src/ft_cmul.c
		libft/src/ft_strrchr.c
		libft/src/ft_wchar_to_string.c
		libft/src/ft_bit_edit.c
		libft/src/ft_putstr.c
		libft/src/ft_atoi.c
		libft/src/ft_strdel.c
		libft/src/ft_atollu_base.c
		libft/src/ft_strnstr.c
		libft/src/ft_strmap.c
		libft/src/ft_lstadd.c
		libft/src/ft_strchr.c
		libft/src/ft_strjoin.c
		libft/src/ft_astr_tolower.c
		libft/src/ft_strstr.c
		libft/src/ft_tpointer_keeper_converter.c
		libft/src/ft_strcpy.c
		libft/src/ft_islower.c
		libft/src/ft_atox_utils.c
		libft/src/ft_isalnum.c
		libft/src/ft_strclr.c
		libft/src/ft_strcmp.c
		libft/src/ft_isascii.c
		libft/src/ft_isdigit.c
		libft/src/ft_toupper.c
		libft/src/ft_memset.c
		libft/src/ft_astr_fill_c.c
		libft/src/ft_atoi_base.c
		libft/src/ft_lstdelone.c
		libft/src/ft_astr_put.c
		libft/src/ft_memdel.c)

add_library(ft_json STATIC ft_json.c)

add_executable(test
		main.c main.c)

target_link_libraries(test ft)