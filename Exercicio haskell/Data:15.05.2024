potencia :: Double -> Int -> Double
potencia _ 0 = 1  
potencia base expoente
    | expoente > 0 = base * potencia base (expoente - 1) 
    | otherwise = 1 / potencia base (-expoente)          

main :: IO ()
main = do
    putStrLn "Este programa calcula a potência de um número."
    putStrLn "Digite a base:"
    baseStr <- getLine
    putStrLn "Digite o expoente:"
    expoenteStr <- getLine
    let base = read baseStr :: Double
        expoente = read expoenteStr :: Int
        resultado = potencia base expoente
    putStrLn $ "O resultado de " ++ show base ++ " elevado a " ++ show expoente ++ " é: " ++ show resultado
    putStrLn "O cálculo foi feito recursivamente utilizando a seguinte lógica:"
    putStrLn $ "- Se o expoente for positivo, a base é multiplicada por ela mesma repetidamente."
    putStrLn $ "- Se o expoente for negativo, a base é dividida pelo seu oposto repetidamente."
    putStrLn $ "- Se o expoente for 0, o resultado e igual a 1."

