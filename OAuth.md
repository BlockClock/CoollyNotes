JSON Web Tokens

格式: xxxxx.xxxxx.xxxxx
称呼: header.playload.sign

加密
header + "." + playload  -> (HMAC SHA-256 算法加密)(base64) = sign