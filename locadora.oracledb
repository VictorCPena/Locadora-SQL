CREATE TABLE clientes (
  id_cliente NUMBER(10) NOT NULL PRIMARY KEY,
  nome_cliente VARCHAR2(50) NOT NULL,
  email_cliente VARCHAR2(50) NOT NULL,
  telefone_cliente NUMBER(12) NOT NULL,
  endereco_cliente VARCHAR2(2100) NOT NULL
);

CREATE TABLE veiculos (
  id_veiculo NUMBER(10) NOT NULL PRIMARY KEY,
  marca_veiculo VARCHAR2(50) NOT NULL,
  modelo_veiculo VARCHAR2(50) NOT NULL,
  ano_veiculo NUMBER(4) NOT NULL,
  tipo_veiculo VARCHAR2(20) NOT NULL
);

CREATE TABLE tarifas_aluguel (
  tipo_veiculo VARCHAR2(20) NOT NULL PRIMARY KEY,
  valor_diaria NUMBER(10,2) NOT NULL
);

CREATE TABLE alugueis (
  id_aluguel NUMBER(10) NOT NULL PRIMARY KEY,
  id_cliente NUMBER(10) NOT NULL,
  id_veiculo NUMBER(10) NOT NULL,
  data_inicio DATE NOT NULL,
  data_fim DATE NOT NULL,
  FOREIGN KEY (id_cliente) REFERENCES clientes (id_cliente),
  FOREIGN KEY (id_veiculo) REFERENCES veiculos (id_veiculo)
);

-- inserindo dados

-- Inserir dados na tabela clientes
INSERT INTO clientes (id_cliente, nome_cliente, email_cliente, telefone_cliente, endereco_cliente)
VALUES (1, 'Patricia Gomes', 'patricia.gomes1@gmail.com', 8599999-9999, 'Vila Velha, 123 - Fortaleza');

INSERT INTO clientes (id_cliente, nome_cliente, email_cliente, telefone_cliente, endereco_cliente)
VALUES (2, 'Savio Laranjeira', 'laranjeirasavio@hotmail.com', 2198888-8888, 'Av. das Palmeiras, 456 - Rio de Janeiro');

INSERT INTO clientes (id_cliente, nome_cliente, email_cliente, telefone_cliente, endereco_cliente)
VALUES (3, 'Claudio Neto', 'claudioneto22@yahoo.com.br', 3197777-7777, 'Rua dos Ipês, 789 - Belo Horizonte');

-- Inserir dados na tabela veiculos
INSERT INTO veiculos (id_veiculo, marca_veiculo, modelo_veiculo, ano_veiculo, tipo_veiculo)
VALUES (1, 'Chevrolet', 'Onix', 2022, 'Hatch');

INSERT INTO veiculos (id_veiculo, marca_veiculo, modelo_veiculo, ano_veiculo, tipo_veiculo)
VALUES (2, 'Fiat', 'Argo', 2021, 'Hatch');

INSERT INTO veiculos (id_veiculo, marca_veiculo, modelo_veiculo, ano_veiculo, tipo_veiculo)
VALUES (3, 'Renault', 'Kwid', 2021, 'SUV');

INSERT INTO veiculos (id_veiculo, marca_veiculo, modelo_veiculo, ano_veiculo, tipo_veiculo)
VALUES (4, 'Volkswagen', 'T-Cross', 2021, 'SUV');

INSERT INTO veiculos (id_veiculo, marca_veiculo, modelo_veiculo, ano_veiculo, tipo_veiculo)
VALUES (5, 'BMW', '330e', 2022, 'Sedan');


-- Inserir dados na tabela tarifas_aluguel
INSERT INTO tarifas_aluguel (tipo_veiculo, valor_diaria)
VALUES ('Hatch', 100);

INSERT INTO tarifas_aluguel (tipo_veiculo, valor_diaria)
VALUES ('SUV', 150);

INSERT INTO tarifas_aluguel (tipo_veiculo, valor_diaria)
VALUES ('Sedan', 200);

INSERT INTO alugueis (id_aluguel, id_cliente, id_veiculo, data_inicio, data_fim)
VALUES (1, 1, 1, TO_DATE('04/03/2023', 'DD/MM/YYYY'), TO_DATE('09/03/2023', 'DD/MM/YYYY'));
INSERT INTO alugueis (id_aluguel, id_cliente, id_veiculo, data_inicio, data_fim)
VALUES (2, 2, 3, TO_DATE('05/03/2023', 'DD/MM/YYYY'), TO_DATE('10/03/2023', 'DD/MM/YYYY'));
INSERT INTO alugueis (id_aluguel, id_cliente, id_veiculo, data_inicio, data_fim)
VALUES(3, 3, 4, TO_DATE('06/03/2023', 'DD/MM/YYYY'), TO_DATE('08/03/2023', 'DD/MM/YYYY'));


