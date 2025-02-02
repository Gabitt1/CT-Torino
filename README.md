import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";

export default function PlayerForm() {
  return (
    <div
      className="flex flex-col items-center justify-center min-h-screen"
      style={{
        backgroundImage: "url('/uploads/Cópia de do dia 29 de janeiro (2).png')",
        backgroundSize: "cover",
        backgroundPosition: "center",
      }}
    >
      <Card className="w-full max-w-3xl shadow-xl border border-gray-300 bg-opacity-90 backdrop-blur-md">
        <CardContent>
          <div className="flex justify-center mb-6">
            <img src="/logo-torino.png" alt="CT Torino Logo" className="h-16" />
          </div>
          <h1 className="text-2xl font-bold text-center text-green-700 mb-6">
            Ficha Técnica - CT Torino
          </h1>
          <form className="space-y-4">
            <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
              <div className="bg-red-900 p-2 rounded">
                <label htmlFor="data_chegada" className="block font-medium text-white font-sans">
                  Data de Chegada:
                </label>
                <input
                  type="date"
                  id="data_chegada"
                  name="data_chegada"
                  className="w-full border border-gray-300 rounded-lg p-2"
                  required
                />
              </div>
              <div className="bg-red-900 p-2 rounded">
                <label htmlFor="nome_completo" className="block font-medium text-white font-sans">
                  Nome Completo:
                </label>
                <input
                  type="text"
                  id="nome_completo"
                  name="nome_completo"
                  className="w-full border border-gray-300 rounded-lg p-2"
                  required
                />
              </div>
              <div className="bg-red-900 p-2 rounded">
                <label htmlFor="data_nascimento" className="block font-medium text-white font-sans">
                  Data de Nascimento:
                </label>
                <input
                  type="date"
                  id="data_nascimento"
                  name="data_nascimento"
                  className="w-full border border-gray-300 rounded-lg p-2"
                  required
                />
              </div>
              <div className="bg-red-900 p-2 rounded">
                <label htmlFor="idade" className="block font-medium text-white font-sans">
                  Idade:
                </label>
                <input
                  type="number"
                  id="idade"
                  name="idade"
                  className="w-full border border-gray-300 rounded-lg p-2"
                  required
                />
              </div>
              <div className="bg-red-900 p-2 rounded">
                <label htmlFor="altura" className="block font-medium text-white font-sans">
                  Altura:
                </label>
                <input
                  type="text"
                  id="altura"
                  name="altura"
                  className="w-full border border-gray-300 rounded-lg p-2"
                  required
                />
              </div>
              <div className="bg-red-900 p-2 rounded">
                <label htmlFor="lateralidade" className="block font-medium text-white font-sans">
                  Lateralidade:
                </label>
                <input
                  type="text"
                  id="lateralidade"
                  name="lateralidade"
                  className="w-full border border-gray-300 rounded-lg p-2"
                  required
                />
              </div>
              <div className="bg-red-900 p-2 rounded">
                <label htmlFor="posicao_1" className="block font-medium text-white font-sans">
                  Posição 1:
                </label>
                <input
                  type="text"
                  id="posicao_1"
                  name="posicao_1"
                  className="w-full border border-gray-300 rounded-lg p-2"
                  required
                />
              </div>
              <div className="bg-red-900 p-2 rounded">
                <label htmlFor="posicao_2" className="block font-medium text-white font-sans">
                  Posição 2:
                </label>
                <input
                  type="text"
                  id="posicao_2"
                  name="posicao_2"
                  className="w-full border border-gray-300 rounded-lg p-2"
                />
              </div>
              <div className="bg-red-900 p-2 rounded">
                <label htmlFor="contato_atleta" className="block font-medium text-white font-sans">
                  Contato do Atleta:
                </label>
                <input
                  type="text"
                  id="contato_atleta"
                  name="contato_atleta"
                  className="w-full border border-gray-300 rounded-lg p-2"
                  required
                />
              </div>
              <div className="bg-red-900 p-2 rounded">
                <label htmlFor="contato_pais" className="block font-medium text-white font-sans">
                  Contato dos Pais:
                </label>
                <input
                  type="text"
                  id="contato_pais"
                  name="contato_pais"
                  className="w-full border border-gray-300 rounded-lg p-2"
                  required
                />
              </div>
              <div className="bg-red-900 p-2 rounded">
                <label htmlFor="cidade_reside" className="block font-medium text-white font-sans">
                  Cidade em que Reside:
                </label>
                <input
                  type="text"
                  id="cidade_reside"
                  name="cidade_reside"
                  className="w-full border border-gray-300 rounded-lg p-2"
                  required
                />
              </div>
            </div>
            <div className="flex justify-center mt-6">
              <Button type="submit" className="bg-green-700 text-white px-6 py-2 rounded">
                Enviar
              </Button>
            </div>
          </form>
        </CardContent>
      </Card>
    </div>
  );
}
